---
layout: post
title: '小呀么小书签'
date: 2009-6-7
wordpress-id: bookmarklets
comments: true
---
什么是小书签？

小书签（Bookmarklet）就是一段JavaScript代码，可以完成特定的功能，你完全可以把它看做是一个链接。

如何使用小书签？

当你看到页面上有“书签工具栏”或者bookmarklet的时候：
<ul>
	<li>Firefox/Chrome/the World：直接拖入书签工具栏</li>
	<li>IE：右键点击，然后选择添加到收藏夹</li>
	<li>Opera：拖到个人栏</li>
</ul>
还是不会的话，可以看看<a href="http://www.douban.com/service/bookmarklet" target="_blank">豆瓣的说明</a>或者<a href="http://xiaonei.com/info/sharehelp.jsp" target="_blank">校内的说明</a>

我的几个小书签(不知道为啥，js不显示完整，所以只提供两个非官方小书签的地址）
<ul>
	<li>Note in Reader：将当前选中内容/当前页面添加到Google Reader的笔记中 官方有</li>
	<li>Bookmark on Delicious：把当前页面收藏到delicious  官方有</li>
	<li>Clip to Evernote：把当前内容收录在evernote里面 官方有</li>
	<li>Add to Reader：将当前站点添加到Google Reader</li>
</ul>
<blockquote>javascript:(function(){for(i=0;i&lt;document.getElementsByTagName('link').length;i++){if(document.getElementsByTagName('link').item(i).getAttribute('rel').toLowerCase()=='alternate' &amp;&amp; (document.getElementsByTagName('link').item(i).getAttribute('type').toLowerCase()=='application/rss+xml' || document.getElementsByTagName('link').item(i).getAttribute('type').toLowerCase()=='text/xml')) { var furl; var fhref=document.getElementsByTagName('link').item(i).getAttribute('href'); if(fhref.indexOf('/')===0) { furl='<a href="http://fusion.google.com/add?1&amp;feedurl='">http://fusion.google.com/add?1&amp;feedurl='</a> + document.location.href.split('/')[0] + '/' + document.location.href.split('/')[1] + '/' + document.location.href.split('/')[2] + fhref; } else if(fhref.indexOf('<a href="http://')===0)">http://')===0)</a> {furl='<a href="http://fusion.google.com/add?2&amp;feedurl='+fhref;">http://fusion.google.com/add?2&amp;feedurl='+fhref;</a> } else { var fhref2=document.location.href.split('/'); fhref2.pop(); furl='<a href="http://fusion.google.com/add?3&amp;feedurl='+fhref2.join('/')+'/'+fhref;">http://fusion.google.com/add?3&amp;feedurl='+fhref2.join('/')+'/'+fhref;</a> } document.location.href=furl;} }})();</blockquote>
<ul>
	<li>Gmail This：用Gmail发送当前选中的内容</li>
</ul>
<blockquote>javascript:(function(){popw='';Q='';x=document;y=window;if(x.selection) {Q=x.selection.createRange().text;} else if (y.getSelection) {Q=y.getSelection();} else if (x.getSelection) {Q=x.getSelection();}popw = y.open('<a href="https://mail.google.com/mail?view=cm&amp;tf=0&amp;to=&amp;su='">https://mail.google.com/mail?view=cm&amp;tf=0&amp;to=&amp;su='</a> + encodeURI(document.title) + '&amp;body=' + encodeURI(Q) + escape('\r') + escape(location.href),'gmailForm','scrollbars=yes,width=680,height=510,top=175,left=75,status=no,resizable=yes');if (!document.all) T = setTimeout('popw.focus()',50);void(0);})()</blockquote>
如果有其他比较好的小书签，欢迎在评论中共享~
