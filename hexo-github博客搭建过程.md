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
	（4）添加图片
		+cd到博客根目录下 查看_config.yml文件 查找 post_asset_folder 字段确定post_asset_folder 设置为true -> post_asset_folder:true
		+当您设置 post_asset_folder 参数后，在建立文件时，Hexo +会自动建立一个与文章同名的文件夹，您可以把与该文章相关的所有资源都放到此文件夹内，这样就可以更方便的使用资源。
		+到博客的根目录下执行 npm install https://github.com/CodeFalling/hexo-asset-image --save 命令来进行插件的安装。
		+然后创建一文章 hexo new "test" 然后查看博客的 ../source/_posts 目录下的文件，会看到存在一个test 文件夹 和 test.md 文件。
		+将所需要的图片资源放到test文件夹内：
		+书写文章使用test文件内 的图片 ![BP](test/BP.png)
		+使用hexo s 命令运行本地博客;
		+使用hexo clean hexo g hexo deploy 将本地博客推送到远程，即可看到文章中的图片。