---
layout:     post
title:      "npm换源与恢复官方源"
subtitle:   "跨平台开发,轻量级桌面应用"
date:       2017-12-03 21:15:06
author:     "CaoZhiLong"
header-img: "img/post-bg-write-with-app-interface-test.jpg"
tags:
    - IDE
    - DeskTop dev
---

# npm换源与恢复官方源

## 引言

&emsp;&emsp;npm,全称Node Package Manager。是node.js的模块依赖管理工具。由于npm 的源在国外，所以国内用户使用起来各种不方便。下面整理出了一部分国内优秀的npm 镜像资源，国内用户可以选择使用。

## 国内优秀npm镜像

**淘宝npm镜像**

&emsp;&emsp;搜索地址：http://npm.taobao.org/

&emsp;&emsp;registry地址：http://registry.npm.taobao.org/

**cnpmjs镜像**

&emsp;&emsp;搜索地址：http://cnpmjs.org/

&emsp;&emsp;registry地址：http://r.cnpmjs.org/

## 如何使用

&emsp;&emsp;有很多方法来配置npm 的registry地址，下面根据不同情境列出几种比较常用的方法。以淘宝npm

镜像举例：
1.**临时使用**

```shell
npm --registry https://registry.npm.taobao.org install express
```

2.**持久使用**

```shell
npm config set registry https://registry.npm.taobao.org

// 配置后可通过下面方式来验证是否成功
npm config get registry

// 或npm info express
```

3.**通过cnpm**
使用

```shell
npm install -g cnpm --registry=https://registry.npm.taobao.org

// 使用cnpm install expresstall express
```
## 如何清除已设置的npm淘宝镜像？

```shell
npm config delete registry

npm config delete disturl

或者 
npm config edit 
找到淘宝那两行,删除
```