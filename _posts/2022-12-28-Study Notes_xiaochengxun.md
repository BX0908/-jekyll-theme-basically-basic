---
layout: page
title: 和风天气小程序2.0
date: 2022-12-28
excerpt_separator: "<!--more-->"
categories:
     - 学习笔记
---

想要拥有属于自己的小程序吗？一起来操作吧

<!--more-->
 
 ![](/assets/images/Study Notes/效果图.png)
 想要实现这样的效果吗？接下来请一起来实操一下

## 请求url
 * key(必选)用户认证key，请参考如何获取你的KEY。支持数字签名方式进行认证。例如 key=123456789ABC
 * location(必选)需要查询地区的LocationID或以英文逗号分隔的经度,纬度坐标（十进制，最多支持小数点后两位），LocationID可通过城市搜索服务获取。例如 location=101010100 或 location=116.41,39.92
  ![](/assets/images/Study Notes/小程序.png)

## 设置data
 ![](/assets/images/Study Notes/data-0.png)
 ![](/assets/images/Study Notes/data-1.png)
 ![](/assets/images/Study Notes/data-2.png)
通过上面的步骤操作下来，我们可以让客户选择想要范访问的地区天气
 ![](/assets/images/Study Notes/选择地区.png)

## 创建一个函数请求和风天气获取这个地址的locationid
 ![](/assets/images/Study Notes/location.png)

## 创建一个函数，里面有我们的wx.request()请求
 ![](/assets/images/Study Notes/request.png)

## 数据渲染
 ![](/assets/images/Study Notes/xuanran.png)


## 设置登录页面效果
 ![](/assets/images/Study Notes/登录1.png)
  ![](/assets/images/Study Notes/登录2.png)
   ![](/assets/images/Study Notes/登录页面.png)

这样大致的和风天气小程序就做出来了，尝试一下效果吧。   


