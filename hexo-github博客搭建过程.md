# hexo-github���ʹ����
�ο���https://www.cnblogs.com/liuxianan/p/build-blog-website-by-hexo-github.html

### 1. ��װNode.js
### 2. ��װGit
### 3. ��װHexo
	��cmd��ִ��npm install hexo-cli -g
	�ȴ���װ��ɺ�����hexo -v����Ƿ�װ�ɹ�
### 4. github���½����Ϳ�username.github.io
### 5. ��ʼ��Hexo
	�½��ļ������ڴ��hexo��ִ��hexo init��
	����hexo����html��css��js���ļ���hexo g
	�������� hexo s����֤�Ƿ����óɹ�
### 6. hexo���⣬�����޸�
	��1����װ���⣨https://hexo.io/themes/��
	git clone https://github.com/iissnan/hexo-theme-next themes/next
	��2���ص�hexo��Ŀ¼�ü��±���_config.xml�ļ����޸�landscape,�ĳ� next��
	��3���޸�_config.yml
		����Site���ݣ�Deployment��Զ�ֿ̲��ַ����
### 7. ����
	��1����װ���𹤾�
		npm install hexo-deployer-git -save
	��2����ʼ�����زֿ�git init
	��4������hexo��github
		hexo clean && hexo g && hexo d
### 8. д����
	��1����λ��hexo��Ŀ¼��ִ�� hexo new ��test��������_posts������md�ļ���
	��2���޸�md�ļ�
		������ʽ��
		---
		title: postName #����ҳ���ϵ���ʾ���ƣ�һ��������
		date: 2013-12-02 15:30:16 #��������ʱ�䣬һ�㲻�ģ���ȻҲ���������޸�
		categories: Ĭ�Ϸ��� #����
		tags: [tag1,tag2,tag3] #���±�ǩ���ɿգ����ǩ���ø�ʽ��ע��:�����и��ո�
		description: ����һ������ժҪ�����������140�����ڣ��������meta��description����
		---

		����������
	��3�����Ĳ���ʾȫ������
		���ں��ʵ�λ�ü���<!--more-->����
		