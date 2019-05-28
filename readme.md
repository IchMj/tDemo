# git
### 版本库
	1.初始化一个版本库 git init (URL) 在当前目录下
	2.git add (file) 可反复添加多个文件
	3.git commit -m <message> 对文件添加注释信息
### 版本控制
	1.修改文件
		- git status 查看仓库当前状态
		- git diff 查看对文件进行了什么修改操作
		最后在进行添加文件
	2.version control
		- git reset --hard HEAD^ 可以回退到上个版本 ^代表一个版本 回退多个版本可以用 HEAD~100表示  
		HEAD 指向的是当前版本 			git reset --head commit id
		- git log 查看历史版本，以便回退到那个版本  --pretty=oneline参数 可以缩略信息
		- git reflog 查看命令历史版本，以便回到未来的那个版本
	3.撤销修改
		- git checkout -- file 撤销工作区修改内容
		- git checkout HEAD <file>撤销缓存区
	4.删除操作
		- git rm <file> 可以删除文件
		- 误删后 可以用 git checkout -- file 进行恢复

