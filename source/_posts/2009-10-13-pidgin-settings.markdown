---
layout: post
title: 'pidgin的设置'
date: 2009-10-13
wordpress-id: pidgin-settings
comments: true
---
这两天开始使用pidgin（windows版），集成了gtalk+qq+msn+飞信。总结一下设置方法：

1.建议语言改为英文的，中文下在修改gtk theme时设置字体程序会崩溃

2.gtalk的账户设置，最好勾选“require ssl/tls”，至于为什么，可以看看<a href="http://initiative.yo2.cn/archives/642153">http://initiative.yo2.cn/archives/642153</a>

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb.png" border="0" alt="image" width="364" height="545" /></a>

3.msn的设置，就用系统内置的msn协议就好，网上大家说的那个比较好的msn-pecan协议经常会导致msvcrt.dll模块崩溃。在教育网的可以勾选“use HTTP method”。同时如果使用NOD32 3版本的话，高级设置按下图修改一下，以免连不上msn，如果<span style="color: #ff0000;">msn报80072745的话，这应该是个比较好的解决方法</span>

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image1.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb1.png" border="0" alt="image" width="370" height="456" /></a>

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image2.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb2.png" border="0" alt="image" width="484" height="348" /></a>

4.QQ用2007或者2008协议都可以登陆，如果不想收到群信息的话，可以取消“Show chat room when msg comes”的选项

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image3.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb3.png" border="0" alt="image" width="415" height="429" /></a>

5.飞信的协议在<a title="http://www.wuala.com/bank000/Setup/libfetion.dll" href="http://www.wuala.com/bank000/Setup/libfetion.dll">http://www.wuala.com/bank000/Setup/libfetion.dll</a>下载，下载后把这个dll放到plugin目录下面。然后在添加飞信协议的时候，如果程序提示说你的手机号码不对（比如是151/152的），<span style="color: #ff0000;">你需要用飞信号和密码登陆</span>。飞信号在用官方客户端里面可以看到。

6.pidgin还可以设置为校内通的客户端。方法是新建一个xampp协议，用户名是校内的ID，也就是你个人主页地址中的id=xxx中的xxx，domain填写为<a href="http://www.renren.com">www.renren.com</a>，高级属性里面服务器选talk.renren.com就能用了。
