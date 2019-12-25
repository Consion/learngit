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