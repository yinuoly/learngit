git config --global user.name"your Name"
git config --global user.name"email@example.com"
注意git config命令的--global参数，用了这个参数，表示你这台机器上所有的Git仓库都会
使用这个配置，当然也可以对某个仓库指定不同的用户名和Email地址

mkdir learngit 创建文件
cd learngit  进入文件
pwd 查看文件的路径
git init 把目录变成git可以管理的仓库

使用Notepad++ 编写文本文件命名 放在learngit目录下
git add 文件名(例如readme.txt) 把文件添加在仓库
git commit -m "wrote a readme file" 把文件提交到仓库
 -m后面输入的是本次提交的说明，可以输入任意内容，当然最好是有意义的 
 
 git status  命令可以让我们时刻掌握仓库当前的状态
 git diff readme.txt 查看修改详情
 git add readme.txt 修改后再提交到仓库
 git status
 git commit -m "add distributed"
 git status
 git add readme.txt
 git log 查看历史记录

修改之后重复如下命令
git add readme.txt
git commit -m "append GPL"

git log 查看历史记录
git log --pretty=oneline

git reset --hard HEAD^ 回退到上一个版本

cat readme.txt 查看文件内容
git log  查看版本库状态
git reset --hard 1094a 指定回到未来的某个版本
cat readme.txt
git reflog 记录之前的命令

git checkout -- readme.txt
命令git checkout -- readme.txt意思就是，把readme.txt文件在工作区
的修改全部撤销，这里有两种情况
git reset HEAD readme.txt
用命令git reset HEAD <file>可以把暂存区的修改撤销掉（unstage），重新放回工作区

rm test.txt 删除没用的文件

是确实要从版本库中删除该文件，那就用命令git rm删掉，并且git commit
git rm test.txt
git commit -m "remove test.txt"



点击“Create repository”按钮，就成功地创建了一个新的Git仓库
git remote add origin (git@github.com:michaelliao/learngit.git)自己文件GitHub地址
git push -u origin master 就可以把本地库的所有内容推送到远程库上
git push origin master 只要本地作了提交，就可以通过命令
