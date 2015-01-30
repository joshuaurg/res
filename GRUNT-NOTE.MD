# LEARN GRUNT S B S
## 基本工作
### windows上下载git客户端，执行linux指令
### 下载node.js.
		node里自带npm,可通过node -v和npm -v查看是否安装成功
### 下载yeoman.
    	npm install -g yo
    	查看是否安装成功？yo -v
### 下载bower.
    	npm install -g bower
    	查看是否安装成功？bower -v
# yeoman实践
## 下载generator
		npm install -g generator-angular<br>
		常见的generator还有webapp，mobile的，格式为generator-[名称]
## 在yo上新建一个angular的项目
		yo angular [项目名称]
		在当前目录下：ls -al,查看生成的项目文件。
# bower实践
		bower install [组件名称]
		执行后，会在当前目录生成一个bower_components文件夹，用于存放下载的组件。
## bower下载分一下几种情况：
* bower install [直接跟组件名称]
* bower install [github短语]。如：bower install jquery/jquery(注册账号/项目)
* bower install [完整的github地址] 。bower install https://github.com/jquery/jquery.git
* bower install [url]。

## bower的两个配置文件：bower.json .bowerrc
* 默认情况下，这两个配置文件是不存在的。

		bower init ---> 生成bower.json
		bower install [名称] --save-dev:下载开发环境所需包
		bower install [名称] --save:下载生产环境所需包
* 手动生成.bowerrc文件并编辑

		{
			"directory":"bower_components",
			"proxy":"http://proxy.tencent.com:8080",
			"https-proxy":"https://proxy.tencent.com:8080",
			"timeout":6000 //单位是毫秒。
		}
		使用代理上网的公司，需要配置代理。

# grunt实践
* 创建一个项目目录并进入
		mkdir grunt-by-yo
		cd grunt-by-yo
* 使用yeoman创建一个webapp项目
		yo webapp [项目名称]
		创建webapp之前，不要忘记安装webapp的generator：npm install -g generator-webapp

















