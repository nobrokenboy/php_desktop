# php_desktop  像开发网站一样开发桌面应用软件
 ![](res/php_desktop.png)
# 特性

1. 支持php的任意版本
2. 支持winxp系统上使用php5.6
3. 支持窗口阴影，皮肤编辑
4. 支持加密数据库，支持sqlite
5. 支持单机、cs模式的软件开发
6. 支持最新版flash
7. 支持窗口间消息通讯
8. 支持窗口运行在子进程
9. 支持PHP错误日志查看
10. 支持启动页面为首页,启动页没有返回操作
11. 支持多workerman服务

# 简要使用说明

1、app目录下是一个单入口PHP项目

2、config.json里配置

    debug: 1开启调试默认 0关闭调试，开启调试后，右键菜单有调试菜单项
    
    url：配置PHP项目启动首页
    
    width：窗口打开的默认宽度，链接打开窗口宽度设置可用window.open传宽度参数
    
    height：窗口打开的默认高度，链接打开窗口高度设置可用window.open传高度参数
    
    title：主窗口打开的标题，其它窗口的标题根据网页titile自动调整
    
    host：如果配置为127.0.0.1，只能本机访问，如果配置为0.0.0.0，则可以局域网访问
    
    web_port：PHP项目访问服务端口号
    
    database：内置数据库相对路径，管理工具tools\数据库查询分析器.exe
    
    data_port：内置数据库访问服务端口号
    
    skin：系统默认皮肤文件，tools\皮肤编辑器.exe可编辑自定义皮肤，群共享里分享了N套皮肤，也可在原有皮肤基础上进行修改
       
    workerman：可启动多个服务，如http,websocket,tcp同时支持
    
        enable：是否启动workerman服务
        
        servers：wokerman服务启动命令列表
        
## 正式发布时建议关闭debug，右键菜单，workerman控制台将隐藏


# 编译步骤
1. delphi 2010
2. 依赖组件 DIOCP5   https://github.com/ymofen/diocp-v5
3. 依赖H5神器组件 OldCEF4Delphi https://github.com/salvadordf/OldCEF4Delphi
4. 依赖装逼UI组件 DynamicSkinForm VCL v1276 http://2ccc.com/article.asp?articleid=6110
5. 依赖组件 Absolute Database v.7.50  ftp://uploads@uploads.2ccc.com/Absolute%20Database%20v.7.50%20-%20Multi-User%20Edition.rar
6. 依赖组件 php4delphi.7.2   https://sourceforge.net/projects/psvlib/files/PHP4Delphi/PHP4Delphi%207.2/
7. 依赖组件 cnvcl  http://www.cnpack.org/showdetail.php?id=830&lang=zh-cn

# FAQ

1. 为什么用delphi编译

答：delphi是开发win32高效工具，编译出来的exe，运行无其它依赖

2. 为什么不用C#

答：C#运行前需要安装.net framework，不能进行绿色发布运行

3. 已经有了nw.js，为什么还需要php_desktop

答：php简单高效，修改代码不需要重启应用，可达到热修复更新系统应用逻辑。目前php_desktop支持界面skin编辑，美观上比nw.js高N个档次

# QQ交流群：423332770
