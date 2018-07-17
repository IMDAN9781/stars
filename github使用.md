# Github日常使用

### 一、配置Git
	1. 在本地创建ssh key 
		$ ssh-keygen -t rsa -C "email@email.com"
		"email@email.com"为github上注册的邮箱，
	    要求确认路径和输入github密码，可用默认。成功后，会再路径下生成.ssh文件夹，进入，打开id_rsa.pub,全选复制内容；
	2. github进入账户配置，选择SSH Keys，将复制的内容贴入；可通过$ ssh -T git@github.com验证是否成功；
	3. 设置username和email
		$ git config --global user.name "your name"
		$ git config --global user.email "email@email.com"

### 二、上传至github仓库
	1. 登录github，新建仓库test；
	2. 要先添加远程地址；
		git remote add origin git@github.com:username/test.git
	3. 在本地新建文件夹，右键使用git bash here，打开git命令行窗口，执行git init；
	4. 将本地文件加入到提交缓冲区，git add * 加全部内容，或指定文件；
	5. 提交文件 git commit -m "提交描述";
	6. 提交到github
		git push origin master
	
### 三、检出仓库
	1. 创建克隆版本
	本地仓库：
		git clone /path/to/repository
	远程仓库：
		git clone username@host:/path/to/repository

### 四、分支
	1. 创建分支"test"并切换过去
		git checkout -b test
	2. 切换或主分支
		git checkout master
	3. 删除分支
		git branch -d test
	4. 删除远程分支
		git push origin :develop-deskmark
	
### 五、更新与合并
	1. 更新只最新版本 
		git pull
	2. 合并其他分支到你当前分支（例如master） 
		git merge <branch>
	3. 查看差异 
		git diff <source_branch> <target_branch>
	
### 六、常见错误
	1. fatal: remote origin already exists.
	解决办法：
		先删除远程git仓库 git remote rm origin（如报错，则手动修改gitconfig文件内容 vi .gt/config，把[remote "origin"]行删除）
		再添加远程git仓库 git remote add origin git@github.com:username/repo
	2. RT ! [rejected] master -> master (fetch first)
	在push远程服务器的时候发现出现此错误；原因是没有同步远程的master
	所以我们需要先同步一下
		git pull origin master
	3. git commit 过程中Changes not staged for commit:
	需要先git add 后在commit 然后 push

	整个流程：
	$ git add menudd //其中 menudd 是一个目录 也可以是文件 会自动更新有修改的文件

	然后 $ git commit -m "asdf" //“asdf”是更新注释

	最后 $ git push origin master

	ok完成 更新成功
