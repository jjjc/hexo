---
title: 利用Hexo搭建博客
date: 2016-09-28 00:24:19
tags:
---
# 一、简述
前不久刚使用hexo搭建了自己博客，hexo是一个静态博客框架使用它可以方便的生成静态网页，同时我们还可以用它托管在github上打造我们自己的专属博客，下面跟着我一起完成一个博客搭建。对了由于我是windows用户，所以下面都是基于windows环境搭建。
<!--more-->
# 二、准备

  要完成我们的目标首先你需要下载并安装
  
- [mysgit](https://git-for-windows.github.io/)
- [Node.js](https://nodejs.org/en/)
> 安装过程默认即可

# 三、正式开始
右键在桌面上单击，然后选择 Git Bush，然后我们安装hexo，输入

![](http://oe64r2af8.bkt.clouddn.com/16-9-27/56467975.jpg)

接下来我们需要在你的想要放的文件夹下新建一个hexo文件夹，用以放博客的文件，进入hexo文件夹，右键单击选择Git Bush，就会创建hexo项目下载所需文件

![](http://oe64r2af8.bkt.clouddn.com/16-9-27/54267976.jpg)

继续我们生成静态页面

![](http://oe64r2af8.bkt.clouddn.com/16-9-27/6778588.jpg)

ok接下来我么可以在本地测试一下到底成功了没，我们输入本地启动命令

![](http://oe64r2af8.bkt.clouddn.com/16-9-27/87582058.jpg)你就可以在浏览器上输入http://localhost:4000/ 看到了

这里我之前不知怎么4000端口被占用了于是我改了下端口就可以了

![](http://oe64r2af8.bkt.clouddn.com/16-9-27/95943930.jpg)


最后不出意外基本上你就可以在本地看到一个不错的博客，当然别人是看不到的。


**也许你还不满意这个博客觉得主题要是可以换个就好了别急我们继续。**

首先先找一个你喜欢的主题，hexo提供[官方地址](http://note.youdao.com/)可以下载一个你比较喜欢的，或者你可以自己在github上找一个非官方的主题下载下来。

我们把下载下来的文件解压缩到hexo/themes下记住文件夹名字或者重新改个，比如叫next。

然后打开我们的hexo文件夹我们发现config.yml的配置文件，我们用记事本打开或者和我一样下载一个Notepad++的文本编辑器，软件小巧但是高效，支持语言也多。找到theme关键字把：后面改成next即可。当然我们还以设置

- 语言 如设置中文： language: zh-Hans具体看你的主题支持哪些。
- 头像 将头像放置主题目录下的 source/uploads/ （新建uploads目录若不存在） 
配置为：avatar: /uploads/头像名.png
- 作者昵称 设置 author 为你的昵称。
等等

在主题的文件夹下面还有一个config.yml,通过修改它我们也可以改变主题的布局等操作。
接下来 我们执行  
```
hexo clean   
hexo g
hexo s
```

就可以在本地查看我们修改的结果了。


下一篇我来谈谈我是如何利用github pages 搭建和托管自己的博客。
