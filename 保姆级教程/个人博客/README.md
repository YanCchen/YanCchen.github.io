## 下载

今天教大家搭建的是个人博客😁，使用的是[**typecho**](http://typecho.org/)博客框架，当然，为了追求好看🤪，使用的主题是[**butterfly**](https://github.com/wehaox/Typecho-Butterfly)

**Typecho完整运行要求：**

> **PHP 5.1以上**

> **Mysql, PostgreSQL, SQLite 任意一种数据库支持，并在PHP中安装了相关扩展**

> **CURL或者Socket扩展支持**

> **mbstring或者iconv扩展支持**

考虑到小白可能不了解PHP，所以本教程使用的是[PHPStudy（小皮）](https://www.xp.cn/download.html)，傻瓜式操作，更简单的搭建个人博客🧐

本次项目需要用到的东西都放在了[下载](../下载/)里，可以自行选择网盘下载🤔

<img src="../下载/YanCchen_2022-08-07_17-41-33.png" height="80px" class="img" />

## 部署环境

**系统：Windows 10 专业版**

**网络环境：内网**

# 部署个人博客

下载好的源码解压(密码是yan)，可以看到以下目录👇

<img src="../img/bmjjc/grbk/ml.png" height="200px" class="img" />

## 安装PHPStudy（小皮）

首先进入**PHPStudy（小皮）**目录，然后解压**phpStudy_64.zip**

<img src="../img/bmjjc/grbk/ml2.png" height="100px" class="img" />

点击**phpstudy_x64_8.1.1.3.exe**，安装PHPStudy（小皮），点击右下角的自定义选项，选择安装位置，我这里安装在E:\PHP\phpstudy_pro

> 尽量不要安装在C盘✌

> 安装路径不能包含中文或空格👌

<img src="../img/bmjjc/grbk/xp1.png" height="200px" class="img" />
<img src="../img/bmjjc/grbk/xp2.png" height="200px" class="img" />

## 部署Typecho

回到目录，解压typecho

<img src="../img/bmjjc/grbk/grbk1.png" height="200px" class="img" />

把解压下来的typecho目录移动到**没有中文或空格的目录下面**，我这里就移动到E盘下

<img src="../img/bmjjc/grbk/grbk2.png" height="150px" class="img" />
<img src="../img/bmjjc/grbk/grbk3.png" height="150px" class="img" />

打开PHPStudy（小皮），启动Apache，可能会出个弹窗，点允许访问就好了👻

<img src="../img/bmjjc/grbk/grbk4.png" height="300px" class="img" />
<img src="../img/bmjjc/grbk/grbk5.png" height="300px" class="img" />

点击左侧的网站，点击里面的管理，修改

<img src="../img/bmjjc/grbk/grbk6.png" height="300px" class="img" />
<img src="../img/bmjjc/grbk/grbk7.png" height="300px" class="img" />

点击浏览，选择你刚刚移动的typecho目录，选择完后确定

<img src="../img/bmjjc/grbk/grbk8.png" height="300px" class="img" />
<img src="../img/bmjjc/grbk/grbk9.png" height="300px" class="img" />

点击首页，启动MySQL,和Apache一样，可能会出个弹窗，点允许访问就好了👽

<img src="../img/bmjjc/grbk/grbk10.png" height="300px" class="img" />
<img src="../img/bmjjc/grbk/grbk11.png" height="300px" class="img" />

点击左侧的数据库，然后点击修改root密码，修改完点击确定就好

<img src="../img/bmjjc/grbk/grbk12.png" height="300px" class="img" />

点击创建数据库，创建一个typecho用的数据库，然后点击确认

> 如果你是放服务器上的，请把你数据库的用户名和密码设置的复杂一点，以免被爆破🤡

<img src="../img/bmjjc/grbk/grbk13.png" height="300px" class="img" />
<img src="../img/bmjjc/grbk/grbk14.png" height="300px" class="img" />

在浏览器打开[http://127.0.0.1](http://127.0.0.1),然后点击下一步

<img src="../img/bmjjc/grbk/grbk15.png" height="300px" class="img" />

输入你刚刚创建的数据库用户名、数据库密码、数据库名，然后点击下一步

<img src="../img/bmjjc/grbk/grbk16.png" height="300px" class="img" />

设置后台管理员的账号、密码、邮箱，然后安装

<img src="../img/bmjjc/grbk/grbk17.png" height="300px" class="img" />

安装完成会提示以下👇

<img src="../img/bmjjc/grbk/grbk18.png" height="250px" class="img" />

然后访问[http://127.0.0.1](http://127.0.0.1)就能看到自己的博客了🤭

<img src="../img/bmjjc/grbk/grbk19.png" height="250px" class="img" />

## 安装butterfly主题

回到目录，进入主题目录，解压**butterfly_Beta1.5.8.zip**

<img src="../img/bmjjc/grbk/zt1.png" height="200px" class="img" />

<img src="../img/bmjjc/grbk/zt2.png" height="200px" class="img" />

然后把刚刚解压的butterfly目录放到typecho\usr\themes里🤥

<img src="../img/bmjjc/grbk/zt3.png" height="200px" class="img" />
<img src="../img/bmjjc/grbk/zt4.png" height="200px" class="img" />

浏览器打开[http://127.0.0.1/admin/](http://127.0.0.1/admin/),输入你之前创建的后台管理账号和密码，登陆🤑

<img src="../img/bmjjc/grbk/zt5.png" height="200px" class="img" />

进入后台，点击左上角的控制台，然后点击外观

<img src="../img/bmjjc/grbk/zt6.png" height="300px" class="img" />

然后找到**Typecho-Butterfly**，点击下面的启用🤨

<img src="../img/bmjjc/grbk/zt7.png" height="300px" class="img" />

然后访问[http://127.0.0.1](http://127.0.0.1)就能看到一个嘎嘎好看的博客啦😍

<img src="../img/bmjjc/grbk/zt8.png" height="300px" class="img" />

到这里就部署完成啦🤗

# 修改个人博客

大部分修改，比如说背景啊，网站图标啊什么的，可以在设置外观里修改🤭

<img src="../img/bmjjc/grbk/zt9.png" height="300px" class="img" />

**更多这个主题的使用介绍请看[typecho-butterfly主题使用文档](https://blog.wehaox.com/archives/typecho-butterfly.html)🤔**

# 关于

### 如果你遇到了什么问题可以通过以下方式来联系我给你解答🤓

> **这里推荐添加QQ群，因为企业微信和邮件不经常看**

***QQ群：[883600025](https://qm.qq.com/cgi-bin/qm/qr?k=geWABzFfMPcFvHQQ4UlZFGji3DSYBQ2p&authKey=DTS5qy7SsNRpmSpSS+3dbX12r7bd/9iZYSJvV4yoZHsz+d8Dpt0bs5dRLK/Y+pdy&noverify=0)***

***企业微信：[点我](https://work.weixin.qq.com/wework_admin/user/h5/qqmail_user_card/vc32c1cd731861b088)***

***邮件：yan@yjf.vin***

***还有网页右边的聊天悬浮窗也可以提问哦👉***
