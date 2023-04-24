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
```
git push --set-upstream origin branch_name：设置本地的branch_name分支对
应远程仓库的branch_name分支
```