# Github日常使用
###一、配置Git
	1. 在本地创建ssh key 
	$ ssh-keygen -t rsa -C "email@email.com"
	"email@email.com"为github上注册的邮箱，要求确认路径和输入github密码，可用默认。成功后，会再路径下生成.ssh文件夹，进入，打开id_rsa.pub,全选复制内容；
	2. github进入账户配置，选择SSH Keys，将复制的内容贴入；可通过$ ssh -T git@github.com验证是否成功；
	3. 设置username和email
	$ git config --global user.name "your name"
	$ git config --global user.email "email@email.com"

###二、上传至github仓库
	1. 登录github，新建仓库test；
	2. 在本地新建文件夹，右键使用git bash here，打开git命令行窗口，执行git init；
	3. 将本地文件加入到提交缓冲区，git add * 加全部内容，或指定文件；
	4. 提交文件 git commit -m "提交描述";
	5. 提交到github， git push origin master（此操作前，需要先添加远程地址执行git remote add origin git@github.com:username/test.git）
	
###三、检出仓库
	1. 创建克隆版本
	本地仓库：git clone /path/to/repository
	远程仓库：git clone username@host:/path/to/repository

###四、分支
	1. 创建分支"test"并切换过去
	git checkout -b test
	2. 切换或主分支
	git checkout master
	3. 删除分支
	git branch -d test
	
###五、更新与合并
	1. 更新只最新版本 git pull
	2. 合并其他分支到你当前分支（例如master） git merge <branch>
	3. 查看差异 git diff <source_branch> <target_branch>
	
	
