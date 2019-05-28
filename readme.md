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
### 关联GitHub
	1.绑定github版本库
		- git remote add origin https://github.com/IchMj/tDemo.git
	2.移除GitHub远程库
		- git remote remove origin
	3.推送本地库到远程
		- git push origin master
	4.从远程克隆库
		- git clone origin https://github.com/IchMj/tDemo.git
### 分支管理
	1.创建分支
		- git branch dev 创建一个dev分支
		- git checkout dev 切换到dev分支
		- git checkout -b dev 相当于上面两条指令
	2.合并分支
		- git merge dev
		- git branch -d dev 删除dev分支
	3.切换分区
		- git checkout <name> 
	4.分支冲突解决
		- 删除分支冲突的内容
