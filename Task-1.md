# �ڦb�o�� task ���z�Ѩ쪺 git �O����F��

-  ��������������n��
-  �i�H�����T�Ӱ϶�
   1. �u�@�ؿ��]Working Directory�^
   2. �Ȧs�ϡ]Staging Area�^
   3. �x�s�w�]Repository�^
## ���O
### directory�]�ؿ��^
- `pwd`�G�d�ݥثe�Ҧb���ؿ�
- `ls`�G�d�ݥؿ������ɮ�
- `cd`�G�ܧ�ؿ�
  - `cd <directoryname>`�G�e���U�@�h�ؿ�
  - `cd ..`�G��^�W�@�h�ؿ�
  - `cd ~`�G��^��l�ؿ�
### repository�]���x�^
- `git clone [url]`�G�N�����W�� repo �U���ܥ��a�q��
- `git init`�G��l�ơ]�إ�`.git`���l��Ƨ��^
### branch�]����^
- `git branch`�G�d�ݩҦ� branch
  - `git branch <new_branchname>`�G�إ߷s�� branch �éR�W
  - `git branch -m <original_branchname> <new_branchname>`�G���s�R�W branch
  - `git branch -d <branchname>`�G�R�����w�� branch
- `git checkout <branchname>`�G�����ܫ��w branch�]�w�]�� `master`�^
  - `git checkout -b <branchname>`�G�إߨä����ܫ��w branch
  - `git diff <branchname1> <branchname2>`�G������ branch �����P���B