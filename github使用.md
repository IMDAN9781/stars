Github�ճ�ʹ��
һ������Git
	1. �ڱ��ش���ssh key 
	$ ssh-keygen -t rsa -C "email@email.com"
	"email@email.com"Ϊgithub��ע������䣬Ҫ��ȷ��·��������github���룬����Ĭ�ϡ��ɹ��󣬻���·��������.ssh�ļ��У����룬��id_rsa.pub,ȫѡ�������ݣ�
	2. github�����˻����ã�ѡ��SSH Keys�������Ƶ��������룻��ͨ��$ ssh -T git@github.com��֤�Ƿ�ɹ���
	3. ����username��email
	$ git config --global user.name "your name"
	$ git config --global user.email "email@email.com"

�����ϴ���github�ֿ�
	1. ��¼github���½��ֿ�test��
	2. �ڱ����½��ļ��У��Ҽ�ʹ��git bash here����git�����д��ڣ�ִ��git init��
	3. �������ļ����뵽�ύ��������git add * ��ȫ�����ݣ���ָ���ļ���
	4. �ύ�ļ� git commit -m "�ύ����";
	5. �ύ��github�� git push origin master���˲���ǰ����Ҫ�����Զ�̵�ִַ��git remote add origin git@github.com:username/test.git��
	
��������ֿ�
	1. ������¡�汾
	���زֿ⣺git clone /path/to/repository
	Զ�ֿ̲⣺git clone username@host:/path/to/repository

�ġ���֧
	1. ������֧"test"���л���ȥ
	git checkout -b test
	2. �л�������֧
	git checkout master
	3. ɾ����֧
	git branch -d test
	
�塢������ϲ�
	1. ����ֻ���°汾 git pull
	2. �ϲ�������֧���㵱ǰ��֧������master�� git merge <branch>
	3. �鿴���� git diff <source_branch> <target_branch>
	
	
