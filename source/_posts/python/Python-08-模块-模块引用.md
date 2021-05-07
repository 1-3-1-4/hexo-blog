---
title: Python--08-模块--模块引用
date: 2021-05-07 18:08:43
tags: [Python, Python学习, Python模块]
categories: Python
description: 模块引用的写法
---



## 一、引入

### 1、`import`语句

在另一个源文件里引入别的模块

`import module1, module2`

### 2、`from ... import ...`语句

`from modname import name1, name2, name3`

### 3、`from ... import *`语句

`from modname import *`

## 二、其他点

### 1、`__name__`属性

一个模块被另一个程序第一次引入时，其主程序将运行。如果我们想在模块被引入时，模块中的某一个程序块不执行，我们可以用 `__name__` 属性来使该程序块仅在该模块自身运行时执行。

```python
#!/usr/bin/python3
# Filename: using_name.py

if __name__ == '__main__':
   print('程序自身在运行')
else:
   print('我来自另一模块')
```

### 2、`dir()`函数

该海曙可以找到模块内定义的所有名称。以一个字符串列表的形式返回：


