git config --global user.name"your Name"
git config --global user.name"email@example.com"
ע��git config�����--global���������������������ʾ����̨���������е�Git�ֿⶼ��
ʹ��������ã���ȻҲ���Զ�ĳ���ֿ�ָ����ͬ���û�����Email��ַ

mkdir learngit �����ļ�
cd learngit  �����ļ�
pwd �鿴�ļ���·��
git init ��Ŀ¼���git���Թ���Ĳֿ�

ʹ��Notepad++ ��д�ı��ļ����� ����learngitĿ¼��
git add �ļ���(����readme.txt) ���ļ�����ڲֿ�
git commit -m "wrote a readme file" ���ļ��ύ���ֿ�
 -m����������Ǳ����ύ��˵�������������������ݣ���Ȼ������������ 
 
 git status  �������������ʱ�����ղֿ⵱ǰ��״̬
 git diff readme.txt �鿴�޸�����
 git add readme.txt �޸ĺ����ύ���ֿ�
 git status
 git commit -m "add distributed"
 git status
 git add readme.txt
 git log �鿴��ʷ��¼

�޸�֮���ظ���������
git add readme.txt
git commit -m "append GPL"

git log �鿴��ʷ��¼
git log --pretty=oneline

git reset --hard HEAD^ ���˵���һ���汾

cat readme.txt �鿴�ļ�����
git log  �鿴�汾��״̬
git reset --hard 1094a ָ���ص�δ����ĳ���汾
cat readme.txt
git reflog ��¼֮ǰ������

git checkout -- readme.txt
����git checkout -- readme.txt��˼���ǣ���readme.txt�ļ��ڹ�����
���޸�ȫ���������������������
git reset HEAD readme.txt
������git reset HEAD <file>���԰��ݴ������޸ĳ�������unstage�������·Żع�����

rm test.txt ɾ��û�õ��ļ�

��ȷʵҪ�Ӱ汾����ɾ�����ļ����Ǿ�������git rmɾ��������git commit
git rm test.txt
git commit -m "remove test.txt"



�����Create repository����ť���ͳɹ��ش�����һ���µ�Git�ֿ�
git remote add origin (git@github.com:michaelliao/learngit.git)�Լ��ļ�GitHub��ַ
git push -u origin master �Ϳ��԰ѱ��ؿ�������������͵�Զ�̿���
git push origin master ֻҪ���������ύ���Ϳ���ͨ������
