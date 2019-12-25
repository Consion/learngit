1. 每个机器都要自报家门，配置名字和邮件地址
git config --global user.name "Your Name"
git config --global user.email "email@example.com"

2.初始化git仓库
git init

3.添加新的文件到git中
git add readme.txt [file2.txt file3.txt]

git commit -m "wrote a readme file."

4.比较文件和版本的不同，并查看状态
git diff readme.txt
git status

5.通过git log来查看提交履历
git log

测试版本回退的内容
6.版本回退
git reset --hard HEAD^  恢复到上一版本
git reset --hard HEAD^^恢复到上上版本
git reset --hard 1094a 恢复到指定commit id版本

7.查看每次的提交履历
git reflog

8.工作区（Working Directory)，就是能看到的目录。

9.版本库（Repository），工作空间中有一个.git隐藏目录，为版本库，主要存放以下内容：
	a.stage（index）的暂存区
	b.git为我们创建的第一个master分支，及指向master分支的HEAD指针
工作目录中的文件通过git add命令来放入到暂存区，然后通过git commit命令来将暂存区中的更改提交到当前分支上。

测试git暂存区的概念
测试git暂存区的概念2
通过对一个文件的修改，第一次执行git add .，第二次直接git commit，执行git status发现文件还是为modifiy状态，发现git add .是把文件的修改
增加到暂存区中，git Commit命令是将暂存区中的更改提交到分支中。

使用git diff HEAD -- readme.txt
	