# git笔记

git 常用命令

**设置提交代码时的用户信息**
```
git init

git config --global user.name "yourUserName"     # 去掉 --global 就只对当前仓库生效

git config --gloabl user.email "yourEmail"       # 去掉 --global 就只对当前仓库生效
```

**日常coding工作流**
```
git add .       ：将当前目录加入到暂存区
git status       
git commit -m  "：给自己看的备注信息"：       将暂存区的内容提交到当前分支
git log         ：查看当前分支的所有版本
git diff        ：比对和暂存区或者最后提交的差别  
git ls-files    ：查看暂存区文件
git rm a.txt   ：将a.txt从工作区和暂存区同时删掉
git rm --cached a.txt   仅从暂存区删掉 -f强制
```

***
**分支操作**
```
git branch          ：查看分支
git checkout -b "分支名"  ：基于当前分支创建一个新分支
git checkout master ：切换分支
git branch -d "分支名"  ：删除分支
git merge branch_name：将分支branch_name合并到当前分支上
```

**远程仓库**

ssh
检查有没有ssh
`cd ~/.ssh && ls`
如果没有 SSH Key，就要输入以下命令行生成：
`ssh-keygen -t rsa -C "这里输入你在 GitHub 的注册邮箱"`

```
将本地代码推送到远程指定分支
git push origin <指定的分支名> -f  // -f加上就是强制 -d可以删除远程分支
git push origin dev:master  

git pull origin main:master
来拉取并合并远程的main分支到本地的master分支

从远程指定分支上拉取代码
git clone -b  <指定分支名>  <ssh或者http地址>

如果第一次create远程的git仓库，将本地与仓库和远程仓库联系
git remote add origin <远程仓库ssh或者http地址>



```

**代码回滚**
```
git reset --hard HEAD^ 或git reset --hard HEAD~ ：将代码库回滚到上一个版本
git reset --hard HEAD^^：往上回滚两次，以此类推
git reset --hard HEAD~100：往上回滚100个版本
git reset --hard 版本号：回滚到某一特定版本
```
