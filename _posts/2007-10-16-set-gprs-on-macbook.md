---
layout: post
title: "苹果笔记本电脑MacOSX系统下. 设置GPRS简要流程"
date: 2007-10-16 12:21
category: "分享"
tags: [软件]
---
{% include JB/setup %}

----------------

应邀MACFANS的网友. 介绍一下我在PB小飞机下的设置 PB+蓝牙+GPRS+手机(SAGEM X8) 的方法:  
[![](http://cache.gizmodo.com/gadgets/images/powerbook_g4.jpg)](http://cache.gizmodo.com/gadgets/images/powerbook_g4.jpg)[![](http://www.mobilewhack.com/images/vectronix_vectrotel_x8_secure_cell_phone.jpg)](http://www.mobilewhack.com/images/vectronix_vectrotel_x8_secure_cell_phone.jpg)  
  
工具条件:  
1.  苹果MAC OSX 系统的笔记本电脑一台. (须具备蓝牙)  
2.  同时支持蓝牙.和GPRS 功能的手机一部  
3.  向移动公司申请开通CMWAP上网包月(或者其他优惠套餐)的手机.SIM卡一张.  
  
流程:  
1.  参考如下网站地址. [http://www.macfans.com.cn/viewthread.php?tid=22114&highlight;=gprs](http://www.macfans.com.cn/viewthread.php?tid=22114&highlight=gprs)  
下载安装和注册 **_GPRS_** Script Generator 这个软件  
2.  使用**_GPRS_** Script Generator 配置你的CMWAP MODERM文件.  
3.  打开手机. 和笔记本的蓝牙.  对你的手机和笔记本进行配对. 在最后一步时注意将. GRRS上网的MODEM配置文件选择为你使用. **_GPRS_** Script Generator 配置那个  
4.  进入  系统预制- 网络 - 蓝牙. 设置你的上网代理为 10.0.0.172:80  
5. -1下载 FIREFOX .上网软件. 并安装.  
   -2 在FIREFOX 地址栏目输入: ababout:config  
          出现列表，找到general.useragent.extra.firefox  
          把字符串值修该为：Nokia（步骤2的目的是修改浏览器的识别，因为中移动对浏览器做了限制）  
   -3  设置.FIREFOX代理. 1firefox 预设－常规－连接设置...－手动配制代理：10.0.0.172 端口：80  
6.  测试. 如果以上没有出现错误...应该能绝对成功!  我本人测试访问成功所有网站. 包括MACFANS. 我的博客. 公会网站. GOOGLE .百度等.全部通过!!!  
  
最后总结, 如果在.GPRS连接网络时鉴定不能通过. 那很可能是你没有正确输入CMWAP帐号.或者没有设置代理.  
如果.你在连接成功.GPRS网络后. 不能打开网页.那肯定是你没有在.FIREFOX中. 设置.general.useragent.extra.firefox为NOKIA的问题.  
  
后记:在苹果电脑下面设置GPRS相对来说.我认为是相当轻松的一件事情.  因为使用苹果的兄弟们都是好心的家伙. 有很多资料可以查询. 如果有问题. 立即使用.GOOGLE搜索.或者到相关论坛发贴(比如MACFANS)找高手帮忙哦  :)



