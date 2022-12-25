---
layout: page
title: HTML基础以及标签
date: 2022-12-25
excerpt_separator: "<!--more-->"
categories:
     - 学习笔记
---

什么是HTML？HTML中有哪些标签？

<!--more-->

## html是世界通用的标记语言，也是一种计算机语言，浏览器能把它翻译并展现出来，用于描述一个网页的信息。

#### 新建的HTML文件中会出现固定起始页面
![](/assets/images/Study Notes/HTML页面.png)
* 一个文档中只会存在一个html、head、body标签
* head: 之间定义，内容可包括标题名、文本文件地址、创作者信息等网页信息说明。head 里面的内容不会在浏览器中显示，它的作用是包含一些页面的元数据
* *head*中可以设置css样式：background、bgcolor、text、link、vlink
* title：定义网页的标题
* meta：说明一些与文档相关的信息，如作者、关键内容、所用语言等
* HTML标记及属性中字母不区分大小写，如<HTML>与<Html>对浏览器来说是完全相同的

#### HTML的常见标签
![](/assets/images/Study Notes/标签.png)
* title标签：< title >< /title >
* div标签：<div></div>
* h标签：h标签中存在六个等级，分别是h1>h2>h3>h4>h5>h6，决定标题的大小

## 新语义标签(节选部分）
* nav: 表示导航
* header: 表示页眉
* footer: 表示页脚
* section: 表示区块
* article: 表示文章 如文章、评论、帖子、博客
* aside: 表示侧边栏 如文章的侧栏
* figure: 表示媒介内容分组 
* mark: 表示标记 
* progress: 表示进度 
* time: 表示日期
* [<font>HTML5所有的标签</font>]( https://www.w3.org/TR/html5/semantics.html#semantics)
