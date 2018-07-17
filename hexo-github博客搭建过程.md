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
	（3）发布hexo到github 
		hexo clean && hexo g && hexo d
### 8. 写博客
	（1）定位到hexo根目录，执行 hexo new “test”，会在_posts下生成md文件；
	（2）修改md文件
		完整格式：
		---
		title: postName #文章页面上的显示名称，一般是中文
		date: 2013-12-02 15:30:16 #文章生成时间，一般不改，当然也可以任意修改
		categories: 默认分类 #分类
		tags: [tag1,tag2,tag3] #文章标签，可空，多标签请用格式，注意:后面有个空格
		description: 附加一段文章摘要，字数最好在140字以内，会出现在meta的description里面
		---

		以下是正文
	（3）博文不显示全部内容：在合适的位置加上<!--more-->即可