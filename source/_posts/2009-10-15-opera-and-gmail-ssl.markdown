---
layout: post
title: 'Opera在教育网下访问gmail的解决方案'
date: 2009-10-15
wordpress-id: opera-and-gmail-ssl
comments: true
---
今天在operachina上闲逛的时候找到的，希望对大家有帮助

如果你是在教育网内，没有开任何出国代理(不是翻墙代理)，那用opera访问gmail的时候，一般都是这样（一直在建立安全连接）

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image4.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb4.png" border="0" alt="image" width="484" height="344" /></a>

但是在同样的网络下，不管是IEFFCHROME都可以访问

<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image5.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb5.png" border="0" alt="image" width="484" height="350" /></a>

一开始我是觉得应该是有一个安全证书在国外，所以如果你只是在教育网的话，没法连接到那个证书去验证，所以最后就超时没法访问了。今天在operachina上看到一个帖子，也是在讨论这个问题，后来有一个人给出了详尽的解决方法：
<ol>
	<li>在Opera里，首选项-安全性-管理证书-证书颁发机构里面，导出Vesign开头的前两个之后，删除掉<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image6.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb6.png" border="0" alt="image" width="484" height="382" /></a></li>
	<li>确定之后重启opera</li>
	<li>接受google和gmail给的证书就ok了，在“安全”里面可以勾选“记住我的选择”<a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image7.png"><img style="border-right-width: 0px; display: inline; border-top-width: 0px; border-bottom-width: 0px; border-left-width: 0px" title="image" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/10/image-thumb7.png" border="0" alt="image" width="484" height="344" /></a></li>
</ol>
问题解决！
