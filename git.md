# git�ʼ�

git ��������

**�����ύ����ʱ���û���Ϣ**
```
git init

git config --global user.name "yourUserName"     # ȥ�� --global ��ֻ�Ե�ǰ�ֿ���Ч

git config --gloabl user.email "yourEmail"       # ȥ�� --global ��ֻ�Ե�ǰ�ֿ���Ч
```

**�ճ�coding������**
```
git add .       ������ǰĿ¼���뵽�ݴ���
git status       
git commit -m  "�����Լ����ı�ע��Ϣ"��       ���ݴ����������ύ����ǰ��֧
git log         ���鿴��ǰ��֧�����а汾
git diff        ���ȶԺ��ݴ�����������ύ�Ĳ��  
git ls-files    ���鿴�ݴ����ļ�
git rm a.txt   ����a.txt�ӹ��������ݴ���ͬʱɾ��
git rm --cached a.txt   �����ݴ���ɾ�� -fǿ��
```

***
**��֧����**
```
git branch          ���鿴��֧
git checkout -b "��֧��"  �����ڵ�ǰ��֧����һ���·�֧
git checkout master ���л���֧
git branch -d "��֧��"  ��ɾ����֧
git merge branch_name������֧branch_name�ϲ�����ǰ��֧��
```

**Զ�ֿ̲�**

ssh
�����û��ssh
`cd ~/.ssh && ls`
���û�� SSH Key����Ҫ�����������������ɣ�
`ssh-keygen -t rsa -C "������������ GitHub ��ע������"`

```
�����ش������͵�Զ��ָ����֧
git push origin <ָ���ķ�֧��> -f  // -f���Ͼ���ǿ�� -d����ɾ��Զ�̷�֧
git push origin dev:master  

git pull origin main:master
����ȡ���ϲ�Զ�̵�main��֧�����ص�master��֧

��Զ��ָ����֧����ȡ����
git clone -b  <ָ����֧��>  <ssh����http��ַ>

�����һ��createԶ�̵�git�ֿ⣬��������ֿ��Զ�ֿ̲���ϵ
git remote add origin <Զ�ֿ̲�ssh����http��ַ>



```

**����ع�**
```
git reset --hard HEAD^ ��git reset --hard HEAD~ ���������ع�����һ���汾
git reset --hard HEAD^^�����ϻع����Σ��Դ�����
git reset --hard HEAD~100�����ϻع�100���汾
git reset --hard �汾�ţ��ع���ĳһ�ض��汾
```
