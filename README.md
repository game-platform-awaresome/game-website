# game-website

#### 程序运行环境 
  1. 系统：windows10   
  2. 环境：node.js环境，MongoDB数据库   
  3. 软件：webstrom，Robomongo

#### 运行方式
1. 运行数据库：   
    * 进入cmd   
    * 进入安装MongoDB的根目录，找到bin文件夹，如cd  e:/MongoDB/bin   
    * 运行以下命令:  mongod –dbpath=e:/gg/db --port=27018        其中e:为项目所在盘   
    * 打开robomongo，点击create，点击save，然后connect

2. 运行项目
    * 进入项目根目录，输入node app，出现数据库连接成功后，视为成功启动项目。


3. 进入项目
    * 打开浏览器，在地址栏输入localhost:8081，即可看到首页。如果没有看到首页，要检查8081端口是否被其他程序所占用。

#### 用户功能
1. 游客通过注册称为网站用户，可以使用前台页面所有功能。  
2. 详细功能：  
    * 首页：查看海报，通过连接跳转到游戏官网  
    * 分类：通过分类查看游戏，点击查看详情进入游戏详情页，可以通过搜索游戏名来查找游戏
    * 论坛：看帖、发帖、发表评论、通过贴名查找帖子  
    * 关于：查看网站相关的信息  
    * 个人信息：查看个人信息

#### 管理员功能
1. 管理员账号：11111111 
2. 管理员密码：123abc  
3. 管理员登陆以后点击管理网站跳到后台页面。role>10为管理员。  
4. 后台模块：  
    * 用户管理：查看用户，删除用户  
    * 游戏管理：    
      * 分类录入  
      + 分类列表：删除分类，修改分类  
      + 游戏录入  
      + 游戏列表：游戏录入，游戏删除  
    * 帖子管理：帖子查看，帖子删除
    
    **数据库文件没有上传，所以管理员账号需要个人手动配置，在数据中写写入一条用户，将它的role设置为大于10的数即可。**
