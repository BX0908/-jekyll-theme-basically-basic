---
layout: page
title: 新手也可以搭建属于自己的个人网站
excerpt_separator: "<!--more-->"
categories:
     - 学习笔记
---
标签: Jekyll Markdown
<!--more-->

## 怎么实现Github+Jekyll 搭建个人网站呢？

#### 使用gitee部署来实现网站搭建（以下为我制作jekyll网站的详细操作）
* ①：拥有一个Gitee和Github账号（分别登录官网）
* ②：找到一个合适的GitHub模板项目，通过fork到自己本地仓库当中
* ③：在Gitee的右上角找到"+"，选择从"Github/GitLab导入仓库"，选中需要导入的仓库进行导入（如图片所示）
* ④：返回代码页面，在_config.yml中修改个人的URL以及baseurl，在页面下面点击提交
* ⑤：注意在_config.yml中要注释掉theme（使用"#"进行注释，并且记得后空一格）起到消除内容的作用
* ⑥：在服务中选择Gitee Pages服务，进行部署（如图片所示）
* ⑦：等待部署，部署成功后出现一条链接

#### 通过以上的操作就成功实现网站的搭建啦，那么接下来就可以开始对自己的个人博客进行内容的丰富和美化！
注意<font color=#FF000 >红色</font>: _Github改动文件后，是自动反应到Page网站上的（可能有延时，或刷新几次网页即可）。但Gitee不是，除非你是Pro版本。Gitee普通版本，需要手工重新部署网站（如图片所示）_
#### 如果在搭建过程中出现问题，可以在网络上寻求帮助
#### [<font>如何搭建个人博客（详细教程）</font>](https://zhuanlan.zhihu.com/p/111832962) 这个链接也可以供大家参考！