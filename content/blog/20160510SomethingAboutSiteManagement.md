+++
title = "建站中的一些问题"
date = 2016-05-10 09:50:20
updated = 2025-02-06 17:00:00
description = ""

[taxonomies]
tags = ["OPS"]

[extra]
quick_navigation_buttons = true
toc = true
mermaid = true

+++

## 概述
 * 主要是为了更好的记录建站中遇到的问题,一方面备忘,一方面来为后来者提供方便

## 问题

### 自定义域名跳转到对应的GitPage页
  * 首先需要在对应的域名解析服务器上添加两条记录如下所示


 记录类型      |     主机记录  | 记录值 
 ------------- | ------------- | -------------
A              |             @ | 192.30.xxx.xxx
A | @ | 192.30.xxx.xxx

  * 在对应的XXX.github.io repository下加入一个以CNAME命名的文件,并在其中写入你的自定义域名如`baidu.com` 切记不要加`www`,之后等待生效即可

### 当发现css js等静态文件加载较慢
 * 这种时候可以使用 七牛等云加速产品来保证网页的加载速度,七牛每个月有一些免费流量,只是有的时候还不如github上的文件加载速度快
 * 更改前端库cdn 为国内的cdn
 * 更改google的字体库位 useso
 * 几个推荐的前端库
  * [BootCDN](http://www.bootcdn.cn/?) 这一个好像就够用了


