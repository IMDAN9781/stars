# egg

## һ����װ
### 1.

## ����egg debug��װ
### 1. VS Code��װdebug
	https://www.debugrun.com/a/9EkVegr.html
	��1����װ��չeggjs
	��2������debug���Խ��棬����launch.json
		{
			"version": "0.2.0",
			"configurations": [{
				"name": "Launch Egg",
				"type": "node",
				"request": "launch",
				"cwd": "${workspaceRoot}",
				"runtimeExecutable": "npm",
				"windows": { "runtimeExecutable": "npm.cmd" },
				"runtimeArgs": [ 
					"run", 
					"debug", 
					"--", 
					"--inspect" 
				],
				"console": "integratedTerminal",
				"protocol": "auto",
				"restart": true,
				"port": 9229,
				"autoAttachChildProcesses": true
			}]
		}
	��3��package.json
		"scripts":{"debug":"egg-bin dev"}
	ע������debug�����ֶϵ��޷����룬��ѯ������ΪVS Code���°汾bug�����ֶ�����auto attach��F1��
	
	����Ϊ"runtimeArgs": ["run","debug", "--", "--inspect"]�����������������޷�debug����Ӧ�õ�һЩ�ϵ㣨���ֶ���auto attach��������Ӧ����"--inspect-bark"(���°汾����ʱ�޷�����)��
### 2. 

##�����ӵ�

##�ġ�
