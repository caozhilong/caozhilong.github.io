---
layout:     post
title:      "前言"
subtitle:   " \"Hello World, 第一篇Blog\""
date:       2015-8-30 13:45:45
author:     "CaoZhiLong"
header-img: "img/post-bg-2015.jpg"
tags:
    - 生活
---

# 前言
> CaoZhiLong的Blog历经波折开通了。
    
之所以说是历经波折，是因为真是费了九牛二虎之力。对于一个对前端一窍不通的人来说，最好的博客是一个傻瓜式，只要写写文档，就能自动生成的工具或者流程。
    当然了，如果样式也漂亮一些，那就更加完美了。
    
> 最开始，我找到了这样的一个[StrayBirds模板](https://github.com/minixalpha/StrayBirds)。如README中所说，这个模板的好处是入手即用，并有多种theme可以选择。    

# Github Pages

github pages是github提供出来的一种托管的页面。因此利用Github Pages来做博客是再合适不过了。更多的帮助可以看[这里](https://help.github.com/categories/github-pages-basics/)。

这里主要介绍一下其中要注意的点。当你github的Repository name是username.github.io时，你的 **master** 分支才是用于生成Github Pages的。
而其生成的页面会直接在根路径下，类似于这样 **http://xuxinkun.github.io/**。

而如果Repository name不是username.github.io，比如[StrayBirds](https://github.com/minixalpha/StrayBirds)，则需要创建 **gh-pages**分支用于自动生成页面。相应的其生成的页面路径也会带有Repository name，类似于 **http://minixalpha.github.io/StrayBirds/** 这样

> Repository name可以在Repository的Settings里修改。

[Huxpro/huxpro.github.io](https://github.com/Huxpro/huxpro.github.io)的直接使用时，最好使用username.github.io的方式来进行使用。不然会有一些路径上的问题，需要自己再进行调整。


# Build

上传好后就github会直接帮你编译。几分钟内就可以在你自己的username.github.io上看到效果了。不过如果想要在本地调试，试看效果的话，可以在本机安装jekyll。

参照[jekyll安装](http://jekyll-windows.juthilo.com/)进行安装。安装完后，在你项目的文件夹直接运行

```
jekyll serve
```

**安装说明**

http://www.tensorfly.cn/bbs/forum.php?mod=forumdisplay&fid=36