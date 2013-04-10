---
layout: post
title: "搭建jekyll博客，和将wordpress备份xml文件转换为markdown数据"
tagline: "wordpress 2 markdown"
description: ""
tags: [学习, 分享]
---
{% include JB/setup %}

本人是个程序白痴，偶然在网上发现了[像黑客一样写博客][1]这篇文章，感觉能够把自己久未更新的博客迁移到[github](http://www.github.com)上面来那就真是太好了，这样做的好处是显而易见的：

* 通过习惯于在linux下面工作和写作，逐渐远离对windows的依赖；
* 拥有一个免费又稳定的静态博客应该是一个很酷的事情，同时，我的文章备份也是非常容易的事；
* 我想学习一些编程方面的知识。

**基于以上几点**开始了漫长的在[fedora 18][2]下面搭建github/+jekyll/+rake/+markdown/+vim的写作环境。当中遇到了很多问题，好在这个星球上有一个强大的发明叫[google](http://www.google.com),总算把博客环境达建好了。在这儿重点记录一下把wordpress数据转换为markdown的问题，以备后面的同学节省一些时间：

1. 首先，需要你的电脑配置好[Python][3]的运行环境；
2. 使用pip安装[wp2md](http://github.com/verygamer/wp2md)

    `pip install -e git+git;//github.com/verygamer/wp2md#egg=wp2md`
    
    
3. 将你的wordpress数据到出为xml文件；
4. 进入你存放xml数据的文件夹，使用如下命令将xml转换为markdown文件（自动分割的）

    `python wp2md.py -d /转换出的md文件目录 你的备份.xml`
    


    
5. enjoy


**更多可以参考wp2md的[README][4]




[1]:http://www.soimort.org/posts/101/
[2]:http://fedoraproject.org/get-fedora
[3]:http://zh.wikipedia.org/wiki/Python
[4]:https://github.com/verygamer/wp2md/blob/master/README.md
