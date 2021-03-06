---
layout:     post
title:      "树原理及相关算法"
subtitle:   "IOS,OpenSource"
date:       2017-12-28 10:15:06
author:     "CaoZhiLong"
header-img: "img/post-bg-write-with-markdown.jpg"
tags:
    - IOS
    - OpenSource
---

# 树原理及相关算法



 &emsp;&emsp;shu对于大量的数据，链表的线性访问时间太慢，不宜使用。我们介绍一种简单的数据结构，其大部分操作的平均时间为
 ```math
 O(log N)
 ```
 。我们还要简述对这种数据结构在概念上的简单修改，保证了在最坏的情况下的上述时间界限。此外，还要学习第二种修改，对于长的指令序列它对每种操作的的运行时间基本上是

  ```math
 O(log N)
 ```

## 学习目标
- 我们涉及到的这种数据结构用于实现几个流行的操作系统的文件系统。
- 看到树如何能够用来计算算术表达式的值。
- 指出如何利用树来支持  ```math O(log N) ```。此外还将学习当数据被保存在磁盘上如何来实现这种操作。

## 预备知识

&emsp;&emsp;树(tree)可以用几种方式定义。

- **递归的方法定义树形结构**

&emsp;&emsp;一棵树是一些节点的集合。这个集合可以是空集；若非空，则一棵树有称作**根(root)**的节点r以及0个或者多个非空的(子树) 组成,$ O(log N) $
```math
  T_{1}  T_{2} …… T_{n}

```
每个子树都被来自根r的一条有向的边连接。每一个子树的根叫做r的儿子(child)，而r是每一颗子树的根的父亲(parent).下图是典型的递归的树

```mermaid
graph TB
 T_{1}-->T_{1}

```




```math

x = a_{1}^n + a_{2}^n + a_{3}^n

x^{y^z}=(1+{\rm e}^x)^{-2xy^w}

J_\alpha(x) = \sum_{m=0}^\infty \frac{(-1)^m}{m! \Gamma (m + \alpha + 1)} {\left({ \frac{x}{2} }\right)}^{2m + \alpha} \text {，行内公式示例}

```