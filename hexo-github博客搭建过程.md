# hexo-github博客搭建过程
参考：https://www.cnblogs.com/liuxianan/p/build-blog-website-by-hexo-github.html

### 1. 安装Node.js
### 2. 安装Git
### 3. 安装Hexo
	打开cmd，执行npm install hexo-cli -g
	等待安装完成后，输入hexo -v检查是否安装成功
### 4. github上新建博客库username.github.io
### 5. 初始化Hexo
	新建文件夹用于存放hexo，执行hexo init；
	加载hexo基础html、css、js等文件：hexo g
	本地启动 hexo s，验证是否配置成功
### 6. hexo主题，配置修改
	（1）安装主题（https://hexo.io/themes/）
	git clone https://github.com/iissnan/hexo-theme-next themes/next
	（2）回到hexo根目录用记事本打开_config.xml文件，修改landscape,改成 next；
	（3）修改_config.yml
		配置Site内容，Deployment（远程仓库地址）；
### 7. 部署
	（1）安装部署工具
		npm install hexo-deployer-git -save
	（2）初始化本地仓库git init
	（4）发布hexo到github
		hexo clean && hexo g && hexo d

		
		
