## 下载

既然我们要搭建个导航页，自己写显然是不大可能的🤣，毕竟时间有限，~~就是因为懒~~，所以我在Github上找到了[EsunR](https://github.com/EsunR)的开源项目

## [Blog-Index](https://github.com/EsunR/Blog-Index)

<img src="../img/bmjjc/dhy/Blog-Index.png" height="400px" class="img" />

**当然考虑到一些小伙伴访问Github速度慢，所以我把源码放在了[下载](../下载/)里**😘

<img src="../下载/YanCchen_2022-08-07_17-41-33.png" height="80px" class="img" />

## 部署环境

**系统：Windows 10 专业版**

**网络环境：内网**

# 部署导航页

我这里以为下载里的源码来进行教程，部署方式都一样，首先解压（密码是yan.vin）,进入目录能看见这些文件

<img src="../img/bmjjc/dhy/mlzs.png" height="250px" class="img" />

## 安装node

首先安装**node**,点进**node**文件，然后双击运行**node-v16.15.0-x64.msi**，**等待一会**

<img src="../img/bmjjc/dhy/node1.png" height="80px" class="img" />

弹出以下窗口，然后开始无脑下一步🤭

<img src="../img/bmjjc/dhy/node2.png" height="200px" class="img" />

## 开始部署

安装好node后开始部署导航页，我这里有无字版和有字版，点击下面的字可以查看无字版和有字版的展示（这里建议如果你用的是logo做图片的话选择无字版，如果用头像的话可以用有字版）

>有字版是在中间的图片下面显示自己设置的字，无字版是把中间图片下面的字给去掉了

> 有字版和无字版部署过程都是一样，所以大家不用担心会不会不一样什么的，看大家喜好自行选择😜

[无字版展示（来自Yan的导航页）](https://yan.vin:86)

[有字版展示（来自原作者的展示）](https://blog-index.vercel.app)

<img src="../img/bmjjc/dhy/dhy1.png" height="200px" class="img" />

我这里选择无字版，点击进入目录，会看到如下文件

<img src="../img/bmjjc/dhy/dhy2.png" height="200px" class="img" /><img src="../img/bmjjc/dhy/dhy3.png" height="200px" class="img" />

点击上方路径栏，输入cmd，然后回车

<img src="../img/bmjjc/dhy/dhy4.png" height="200px" class="img" /><img src="../img/bmjjc/dhy/dhy5.png" height="200px" class="img" />

在命令终端输入npm install，然后回车，安装依赖
```
npm install
```
<img src="../img/bmjjc/dhy/dhy6.png" height="100px" class="img" />

安装完成后，输入npm run build，开始编译
```
npm run build
```
<img src="../img/bmjjc/dhy/dhy7.png" height="100px" class="img" />

编译完成后会发现多了个dist文件

<img src="../img/bmjjc/dhy/dhy8.png" height="200px" class="img" />

<img src="../img/bmjjc/dhy/dhy9.png" height="200px" class="img" />

## 安装IIS服务

> 安装IIS服务，用IIS服务把导航页挂到网上

进入控制模板，然后点击程序

<img src="../img/bmjjc/dhy/IIS1.png" height="200px" class="img" /><img src="../img/bmjjc/dhy/IIS2.png" height="200px" class="img" />

点击启用或关闭Windows功能

<img src="../img/bmjjc/dhy/IIS3.png" height="200px" class="img" />

选择internet information Services,然后点击确定

<img src="../img/bmjjc/dhy/IIS4.png" height="200px" class="img" /><img src="../img/bmjjc/dhy/IIS5.png" height="200px" class="img" />

安装完成，点击重启

<img src="../img/bmjjc/dhy/IIS6.png" height="200px" class="img" />

重启完成后右击此电脑，点击管理

<img src="../img/bmjjc/dhy/IIS7.png" height="200px" class="img" />

按照图片标记的顺序点击

<img src="../img/bmjjc/dhy/IIS8.png" height="200px" class="img" />

然后在右边找到基本设置，点击它，然后点击路径旁边的三个点，选择导航页下的dist文件

<img src="../img/bmjjc/dhy/IIS9.png" height="200px" class="img" />

<img src="../img/bmjjc/dhy/IIS10.png" height="200px" class="img" />

<img src="../img/bmjjc/dhy/IIS11.png" height="200px" class="img" />

选择完后确定

<img src="../img/bmjjc/dhy/IIS12.png" height="200px" class="img" />

打开浏览器，访问[127.0.0.1](http://127.0.0.1)，出现以下界面就没问题了😎

<img src="../img/bmjjc/dhy/dhy10.png" height="200px" class="img" />

> **导航页部署完成**

# 修改导航页

既然都部署，那肯定要改成自己喜欢的啦

这里介绍个命令，**npm run serve**，使用这个命令可以实时刷新你修改的样式

和部署导航页第一步一样，在路径栏里输入cmd回车，然后输入命令npm run serve，然后回车
```
npm run serve
```

<img src="../img/bmjjc/dhy/xg/kfms.png" height="200px" class="img" />

浏览器访问[127.0.0.1:8080](http://127.0.0.1:8080)，就可以看见你导航页了

#### 疑问
**为什么要用这个命令？😦**

> 每次修改，我们都需要通过重新编译(npm run build)才能看到我们修改的内容，很麻烦

> 使用这条命令(npm run serve)可以进行实事刷新你修改的东西,妈妈再也不用害怕我改得不好看了

**我修改完了，我要怎么关闭😮**

> 关掉窗口就好了

**为什么我访问127.0.0.1我修改的东西全部没了😰**

> 因为你没有编译，和部署导航页第一步一样，在路径栏里输入cmd回车，然后输入命令npm run build，然后回车，等加载完就好了

### Notepad++

为了更方便修改，这里建议安装下**Notepad++**，安装方法和node一样，无脑下一步🤭

<img src="../img/bmjjc/dhy/xg/cjjsb.png" height="200px" class="img" />

## 修改这个不知道叫什么

<img src="../img/bmjjc/dhy/xg/bzd1.png" height="200px" class="img" />

进入导航页下的public，右击index.html用Notepad++来编辑它

<img src="../img/bmjjc/dhy/xg/bzd2.png" height="200px" class="img" /><img src="../img/bmjjc/dhy/xg/bzd3.png" height="200px" class="img" />

我这里画了个图，应该比较好理解

<img src="../img/bmjjc/dhy/xg/bzd4.png" height="300px" class="img" />

> 这里提醒以下，那个图片名称必须是**favicon**，后缀必须是**ico**

## 导航页中间的图片

<img src="../img/bmjjc/dhy/xg/logo.png" height="200px" class="img" />

进入导航页下的\src\assets，里面logo.svg就是这个图片了

> 这个和上面那个一样，名字必须是logo，后缀必须是svg

<img src="../img/bmjjc/dhy/xg/logo2.png" height="200px" class="img" />

## 其他修改

进入导航页下的src，这里有一个config.js文件，基本的设置都在这个文件里，右击用Notepad++来编辑它

> 这里基本都有注释，我就不一一介绍了，我这里介绍一些如何新增或减少导航的分类和标题

<img src="../img/bmjjc/dhy/xg/qtxg1.png" height="400px" class="img" />

还有上面没画到的
```
pageId: 1,
sortId: 1,
```
这个是什么，各位有没有注意到标题分类1和标题分类2，前面的sortId: 1和sortId: 2🤔

<img src="../img/bmjjc/dhy/xg/qtxg2.png" height="400px" class="img" />

然后再看上一个图的分类是什么，想必应该会怎么修改了吧，嘿嘿嘿🤤

### 新增分类这里要注意

一个是前面的数字，不能重复，你可以用其他数字，但就是不能重复

<img src="../img/bmjjc/dhy/xg/qtxg3.png" height="200px" class="img" />

最后面是不用加英文,的，但前面的必须加，不然就是

**错误警告！！！😲**

<img src="../img/bmjjc/dhy/xg/qtxg4.png" height="400px" class="img" />

给前面加了英文,后恢复正常😯

<img src="../img/bmjjc/dhy/xg/qtxg5.png" height="400px" class="img" />

## 关于

### 如果你遇到了什么问题可以通过以下方式来联系我给你解答🤓

> **这里推荐添加QQ群，因为企业微信和邮件不经常看**

***QQ群：[883600025](https://qm.qq.com/cgi-bin/qm/qr?k=geWABzFfMPcFvHQQ4UlZFGji3DSYBQ2p&authKey=DTS5qy7SsNRpmSpSS+3dbX12r7bd/9iZYSJvV4yoZHsz+d8Dpt0bs5dRLK/Y+pdy&noverify=0)***

***企业微信：[点我](https://work.weixin.qq.com/wework_admin/user/h5/qqmail_user_card/vc32c1cd731861b088)***

***邮件：yan@yjf.vin***

***还有网页右边的聊天悬浮窗也可以提问哦👉***