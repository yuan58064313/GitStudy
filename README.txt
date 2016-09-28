2016-9-27
lxiao
--------------------------------------------------
安装与配置
	centos安装Git
	配置Git
$ git config --global user.name "My Name" 
$ git config --global user.email myEmail@example.com
--------------------------------------------------
新建一个Git仓库
	创建目录:
$ mkdir ~/Git
	进入目录:
$ cd ~/Git
	初始化你的新Git工作区:
$ git init
	编写一个文件:
$ echo "hello world" > sample.c
	查看状态:
$ git status
	add命令:
$ git add sample.c
	提交目录下的所有内容:
$ git add -A

$ git status
	撤销:
$ git reset HEAD sample.c
	commit, -m "":表示对这次提交的描述，建议使用有意义的描述性信息。
$ git commit -m 'My great project, fist commit.'	
	log:
$ git log --oneline
$ git log
--------------------------------------------------
远程仓库
	链接远端仓库 - git remote add
$ git remote add origin https://github.com/tutorialzine/awesome-project.git
	上传到服务器 - git push
$ git push origin master
	- git clone
$ git clone https://github.com/tutorialzine/awesome-project.git
	- git pull
$ git pull origin master
--------------------------------------------------
