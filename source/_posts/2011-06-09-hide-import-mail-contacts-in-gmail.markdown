---
layout: post
title: '隐藏Gmail导航栏中的"import mail & contacts"'
date: 2011-6-9
wordpress-id: hide-import-mail-contacts-in-gmail
comments: true
---
浏览器是Firefox

在AdBlock Plus里面加入两条：
<blockquote>mail.google.com##span.Qx
mail.google.com##span.Pn</blockquote>
或者修改userContent.css（在profile文件夹\chrome\userContent.css，如果没有该文件夹就新建一个），添加：
<blockquote>@-moz-document domain(mail.google.com) {
/* hide new red labels */
span.Qx, span.Pn {
display: none !important;
}
}</blockquote>
<a href="http://www.google.com/support/forum/p/gmail/thread?tid=28abbd5f0a113dc9&amp;hl=en" target="_blank">via </a>

P.S.：minimalist Gmail在不同分辨率下的表现不一样？我在笔记本上（1024×768）可以完全隐藏导航栏，在台式机上（1280×1024）就不可以，剩这么一个import mail &amp; contacts在外面
