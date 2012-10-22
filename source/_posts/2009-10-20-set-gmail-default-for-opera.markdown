---
layout: post
title: 'Opera使用gmail作为默认邮件发送工具'
date: 2009-10-20
wordpress-id: set-gmail-default-for-opera
comments: true
---
<p>在用opera浏览网页的时候，如果点了一个mailto的链接，很可能跳出来的是outlook Express或者ms outlook。如何设置opera才能让写邮件默认调用网页版gmail呢？</p>  <p>1.在Opera安装目录\default下，修改webmailproviders.ini文件，添加以下几句：</p>  <blockquote>   <p>[Gmail This!]      <br />ID=3       <br />URL=<a href="https://mail.google.com/mail?view=cm&amp;tf=0&amp;to=%t">https://mail.google.com/mail?view=cm&amp;tf=0&amp;to=%t</a>      <br />ICON=http://mail.google.com/favicon.ico</p> </blockquote>  <p>其中ID随你设置为多少</p>  <p>2.然后在Opera的首选项-高级-程序里面，把mailto协议改为Gmail This</p>  <p><a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image8.png"><img style="border-bottom: 0px; border-left: 0px; display: inline; border-top: 0px; border-right: 0px" title="image" border="0" alt="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb8.png" width="484" height="376" /></a>&#160; </p>  <p><a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image9.png"><img style="border-bottom: 0px; border-left: 0px; display: inline; border-top: 0px; border-right: 0px" title="image" border="0" alt="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb9.png" width="454" height="468" /></a> </p>  <p>以后点击mailto的链接的时候，直接就会跳出gmail写信的窗口了</p>
