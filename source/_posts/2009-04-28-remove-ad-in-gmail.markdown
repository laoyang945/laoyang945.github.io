---
layout: post
title: '如何去除gmail中的广告？'
date: 2009-4-28
wordpress-id: remove-ad-in-gmail
comments: true
---
<p>今天和大家分享一个小技巧，如何移除gmail右侧的广告？</p>
<p>如果你使用客户端处理gmail邮件的话，那不用看接下来的内容了，用客户端没有广告。</p>
<p>我说的广告，是指下图中的红框部分，因为本来笔记本的分辨率就小（1024），再加上我把标签栏移到了右边，要是还有广告的话，正文会显得十分拥挤：</p>
<p><a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/04/image3.png"><img style="border-top-width: 0px; display: inline; border-left-width: 0px; border-bottom-width: 0px; border-right-width: 0px" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/04/image-thumb3.png" border="0" alt="image" width="484" height="218" /></a></p>
<p>移除这个广告的方法，主要是用user css，或者是user js</p>
<p><!--more--></p>
<ul>
<li>如果你是Opera或者Firefox的用户，可以直接用样式表来修改（Firefox需要安装插件stylish)。</li>
</ul>
<p>新建一个gmail-removeAD.css的文件，用文本编辑器便器，使内容是：</p>
<p>==================以下代码开始======================</p>
<blockquote><p>/*加大正文字体及行高*/<br />
.ii.gt,.ii.gt *{font-size:14px !important;line-height:1.5 !important}<br />
/*隐藏读信广告*/<br />
table.T1HY1.nH.iY{width:100% !important;}<br />
table.Bs.nH.iY td.Bu:last-child{display:none;}<br />
/*下面是把快速动作栏隐藏起来了，如果你需要的话，去除从position到important的注释，并且删除display:none这一句*/<br />
table.T1HY1.nH.iY td.tELAdc:last-child{/*position:absolute !important;top:-65px !important;left:0 !important;*/display:none}<br />
table.T1HY1.nH.iY td.tELAdc:last-child .nH{width:auto !important}<br />
table.T1HY1.nH.iY td.tELAdc:last-child .hk{float:left !important;margin-left:1em !important;}<br />
/*这一句是隐藏邀请朋友框*/<br />
.nH.pp.ps .pY{display: none !important;}</p></blockquote>
<p>=================以上代码结束======================</p>
<p>然后在浏览器中对gmail使用这个样式表就行了，下面是使用之后的截图，是不是清爽了很多？</p>
<p><a href="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/04/image4.png"><img style="border-top-width: 0px; display: inline; border-left-width: 0px; border-bottom-width: 0px; border-right-width: 0px" src="http://laoyang.yo2.cn/wp-content/uploads/300/30018/2009/04/image-thumb4.png" border="0" alt="image" width="484" height="224" /></a></p>
<ul>
<li>如果你是Chrome的用户，并且是2.0之后的版本，可以用userjs来处理。新建一个叫做gmail.user.js的文件，用文本编辑器打开，然后其内容是</li>
</ul>
<blockquote><p>// ==UserScript==<br />
// @name          GMail - Remove ads and relocate action links<br />
// @namespace     <a href="http://userstyles.org">http://userstyles.org</a><br />
// @description      This style removes the ad panel from Gmail or Google Apps Mail, relocates the action links (Print all, new window, etc.) from the side bar to above the mail subject, and widens the mail content area<br />
// @author        lOtR<br />
// @homepage      <a href="http://userstyles.org/styles/11768">http://userstyles.org/styles/11768</a><br />
// @include       <a href="http://mail.google.com/*">http://mail.google.com/*</a><br />
// @include       <a href="https://mail.google.com/*">https://mail.google.com/*</a><br />
// @include       <a href="http://*.mail.google.com/*">http://*.mail.google.com/*</a><br />
// @include       <a href="https://*.mail.google.com/*">https://*.mail.google.com/*</a><br />
// ==/UserScript==<br />
(function() {<br />
var css =".ii.gt,.ii.gt *{font-size:14px !important;line-height:1.5 !important;}table.T1HY1.nH.iY{width:100% !important;}table.Bs.nH.iY td.Bu:last-child{display:none !important;}table.T1HY1.nH.iY td.tELAdc:last-child .nH{width:auto !important}table.T1HY1.nH.iY td.tELAdc:last-child .hk{float:left !important;margin-left:1em !important;}.nH.pp.ps .pY{display: none !important;}";<br />
if (typeof GM_addStyle != "undefined") {<br />
GM_addStyle(css);<br />
} else if (typeof addStyle != "undefined") {<br />
addStyle(css);<br />
} else {<br />
var heads = document.getElementsByTagName("head");<br />
if (heads.length &gt; 0) {<br />
var node = document.createElement("style");<br />
node.type = "text/css";<br />
node.appendChild(document.createTextNode(css));<br />
heads[0].appendChild(node);<br />
}<br />
}<br />
})();</p></blockquote>
<p>将这个脚本放入目录 C:\Documents and Settings\{username}\Local Settings\Application Data\Google(Chromium)\Chrome\User\ DataDefault\User Scripts 下。</p>
<p>修改chrome快捷方式的属性，使其能使用userjs，比如这样的"C:Documents and Settings{username}Local SettingsApplication DataGoogleChromeApplicationchrome.exe" --enable-user-scripts。</p>
<p>另外，Google不好的一点是，在搜索的结果里面，会加入一个重定向的功能，也就是如果你登陆了gmail，在你点击搜索结果的时候，为了能记录你的浏览历史，google会把网址变为<a href="http://www.google.com/url?sa=U&amp;start=1&amp;q">http://www.google.com/url?sa=U&amp;start=1&amp;q</a>=……这样的形式，有时候你访问被墙的东西时，整个google就会被封掉……。解决办法是用一个user js，内容很简单</p>
<blockquote><p>// ==UserScript==<br />
// @include       <a href="http://www.google.com/search?*">http://www.google.com/search?*</a><br />
//<br />
// ==/UserScript==</p>
<p>var linkList = document.getElementById("res").getElementsByTagName("a");<br />
for(var i = 0; i &lt; linkList.length; i++) {<br />
var link = linkList[i];<br />
link.setAttribute('onmousedown',null);<br />
}</p></blockquote>
<p>这篇日志参考了<a title="http://ytzong.blogspot.com/2009/03/stylishgmail.html" href="http://ytzong.blogspot.com/2009/03/stylishgmail.html">http://ytzong.blogspot.com/2009/03/stylishgmail.html</a>和<a title="http://zhiqiang.org/blog/posts/enable-userscripts-chrome-gmail.html" href="http://zhiqiang.org/blog/posts/enable-userscripts-chrome-gmail.html">http://zhiqiang.org/blog/posts/enable-userscripts-chrome-gmail.html</a></p>
