# egg

## 一、安装
### 1.

## 二、egg debug安装
### 1. VS Code安装debug
	https://www.debugrun.com/a/9EkVegr.html
	（1）安装扩展eggjs
	（2）进入debug调试界面，配置launch.json
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
	（3）package.json
		"scripts":{"debug":"egg-bin dev"}
	注：启动debug，发现断点无法进入，查询到可能为VS Code的新版本bug，需手动开启auto attach（F1）
	
	配置为"runtimeArgs": ["run","debug", "--", "--inspect"]可正常启动，但是无法debug启用应用的一些断点（需手动加auto attach）。正常应该用"--inspect-bark"(但新版本配置时无法启动)。
### 2. 

##三、坑点

##四、
