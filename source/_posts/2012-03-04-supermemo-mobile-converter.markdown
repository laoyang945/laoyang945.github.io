---
layout: post
title: "Supermemo iPhone版课程生成脚本"
date: 2012-03-04 14:20
comments: true
categories: [English learning, python]
---

老婆要从头开始准备考雅思了，我先找了一本李笑来的《[新托福iBT词汇分类突破][1]》（感谢作者自己提供[PDF版本下载][2]）来给她背单词，里面的插画十分有爱。学习的劲头也被点燃了，我现在每次回家都看见她在看这本单词书（怎么和我电脑屏幕总是桌面一个感觉）。

但是准备过这种考试的都知道，背单词主要是在重复，一开始能记住基本是没用的，而且是有策略的重复，一次记不住单词的意思不要紧，先往前走，把能记住的记住了，记不住的反复记。原来我自己准备GRE的时候自己是弄了一个时间表，哪一天背哪几个新的单词表，复习哪几个旧的都列在上面，严格按照这个时间表来进行，最后效果也比较满意。

我一直在订阅舍得的博客，里面介绍了不少supermemo的用法。于是我就想用supermemo辅助我老婆的记单词任务。简单搜索了一下，发现supermemo有iOS的版本，还是免费的，正好家里面也有iPad和iPod Touch可以直接使用。原来我安卓上的那个Anki记忆软件在App Store里面要24.99美金，于是放弃了。

下载之后发现Supermemo iPhone版之所以是免费的，因为他里面的很多课程都需要用户购买。不过他也提供了自定义课程的功能。可以直接把你需要的问题/答案写在一个特定格式的文本文件里，上传到设备进行学习。那于是我就在想怎么能把李笑来这本书里面的单词做成一个课程，甚至把任意的单词表生成课程。

在[这个项目][3]的启发下，我自己也写了一个Python脚本，能够把utf-8编码并用tab键分开的的txt文档转换为supermemo可以导入的格式。项目链接在[这里][4]，这还是我第一次用github发布自己的代码。

使用方法,运行即可,会要求输入源文件路径及各列编号:

<img src="https://lh6.googleusercontent.com/-_qYA21fdGB4/T1MKDpH8PHI/AAAAAAAAbJc/qYS6IyN-tTg/2012-03-04%25252014%25252018%25252013.png" width="500" />

源文件必须要用Tab分隔，音标暂时只能处理金山词霸的：

<img src="https://lh5.googleusercontent.com/-3uxYo6zD8LY/T1MKDgPndtI/AAAAAAAAbJk/08b7N86DQDA/2012-03-04%25252014%25252018%25252038.png" width="500" />

输出文件内容:

<img src="https://lh4.googleusercontent.com/-s-TxAUPjhd4/T1MKDp-qLCI/AAAAAAAAbJg/MXHCsBnMaoY/2012-03-04%25252014%25252018%25252048.png" width="500" />

iOS设备效果：

<img src="https://lh6.googleusercontent.com/-qE6IPfRHROE/T1MLEtkYq9I/AAAAAAAAbJ0/lVWrO1e-i40/%2525E7%252585%2525A7%2525E7%252589%252587.PNG" width="500" />

[1]: http://www.lixiaolai.com/archives/8079.html
[2]: http://www.lixiaolai.com/archives/11089.html
[3]: http://github.com/tikiet/sm_iphone_qa_generator
[4]: http://github.com/laoyang945/supermemo-mobile-converter
