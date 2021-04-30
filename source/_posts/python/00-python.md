---
title: Python--前言
date: 2021-04-24 16:30:52
tags: [Python, Python学习]
categories: Python
description: 了解Python
---

## 先了解python

### 1、python是一种解释性语言

python也是需要编译的，只不过Python不像java那样需要去强编译「手动编译」，Python在执行时是自动完成编译。

编译的结果是保存于在位于内存中的**PyCodeObject**中，然后通过解释器将PyCodeObject写回到**pyc**文件中。

当Python程序第二次运行时，首先会在硬盘中找pyc文件，如果找到直接载入，没有就执行正常过程。

> 编译型语言C语言，就需要一个编译的过程，把程序转成机器语言。

### 2、pyc文件生成的位置

会在生成在执行文件的同级，生成在默认的目 `__pycache__`下面，如果`import`的文件的名字为`example`，生成的名字格式大概为`example-cpython-39.pyc`。

### 3、pyc文件有效性

python每次载入pyc文件之前会检查下py文件和pyc文件的最后修改日期，如果日期不一致会重新生成一份pyc文件



## 优缺点

### 1、优点

1、python有许多完善的基础代码库，开发时实用很方便

### 2、缺点

1、代码不能加密，因为Python是解释性语言，源代码是以明文形式存放，如果项目有对代码加密的需求，不要用Python来实现



#### <!--深入的遇到再补充-->