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
	��1����װ����
	git clone https://github.com/iissnan/hexo-theme-next themes/next
	��2���ص�hexo��Ŀ¼�ü��±���_config.xml�ļ����޸�landscape,�ĳ� next��
	��3���޸�_config.yml
		����Site���ݣ�Deployment��Զ�ֿ̲��ַ����
### 7. ����
	��1����װ���𹤾�
		npm install hexo-deployer-git -save
	��2����ʼ�����زֿ�git init
	��4������hexo��github
		hexo clean && hexo g && hexo -d

		
		