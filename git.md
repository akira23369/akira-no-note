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
```
git push --set-upstream origin branch_name�����ñ��ص�branch_name��֧��
ӦԶ�ֿ̲��branch_name��֧
```