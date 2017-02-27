##npm && nrm && bower

##npm
>npm是后端的nodejs包构建工具

####npm全局安装 与 本地安装的区别
- 全局安装（只在命令下使用）
    - nrm 工具（切换镜像源地址）
    ```npm install nrm -g```
    - bower （前端模块管理工具）
    ``` npm install bower -g``` 
    - jade （后端模板引擎）
    ```npm install jade -g```
    - webpack （项目构建化工具）
    ```npm install webpack -g ```
    - .....
-  本地安装
	- 项目模块 
	```npm install [modelName] [options]```
    - 依赖（开发上线都需要）
    ```npm install jquery --save```
    - 开发依赖（只在开发使用）
    ```npm install jquery --save-dve```
    
####npm命令
- ```npm config ls```  查看npm的配置信息。
- ```npm init``` 初始化一个npm项目 会在当前文件夹生成一个json配置文件。
- ```npm adduser``` 注册一个用户，输入用户名，输入密码，等信等息进行注册，注册成功会自动登录npm官网。
- ```npm install jquery```  从npm官网中下拉一个第三方模块。
- ```npm update [name] ```升级一个包。
- ```npm uninstall [name]``` 卸载一个包。
- ```npm publish``` 发布一个包
- ```npm -d install [name]``` 表示安装时显示进度。
- ```npm list --depth 0``` 查看本地的npm包。
- ```npm info jquery``` 查看版本
- ```npm list -g --depth 0```查看全局的npm包。

##bower
- bower安装指令 ```bower install jquery --save ``` 和```npm```用法指令一样
- bower安装的模块路径，默认安装到bower_components文件夹中
- 指定bower的安装路径,新建一个.bowerrc文件 写入 ```{"directory":"目录地址"}``` bower会自动识别该文件。
- bower指令
	- ```cache```:bower缓存管理
	- ```help```:显示Bower命令的帮助信息
	- ```home```:通过浏览器打开一个包的github发布页
	- ```info```:查看包的信息
	- ```init```:创建bower.json文件
	- ```install```:安装包到项目
	- ```link```:在本地bower库建立一个项目链接
	- ```list```:列出项目已安装的包
	- ```lookup```:根据包名查询包的URL
	- ```prune```:删除项目无关的包
	- ```register```:注册一个包
	- ```search```:搜索包
	- ```update```:更新项目的包
	- ```uninstall```:删除项目的包	 

##nrm
- nrm是npm源镜像管理工具
- nrm的命令
	- ```npm install nrm -g```下载
	- ```nrm ls```查看所有源
	- ```nrm test```查看源速度
	- ```nrm add 源名字 源地址```添加源
	- ```nrm del 源名字```删除源
	- ```nrm use 源名字```使用源