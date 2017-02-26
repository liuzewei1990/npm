##npm笔记
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