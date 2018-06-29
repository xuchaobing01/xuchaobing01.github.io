---
layout:     post
title:      "Linux 命令行 光标移动技巧"
subtitle:   "看一个真正的专家操作命令行绝对是一个极好的体验！"
date:       2018-06-29 10:00:00
author:     "Sean"
header-img: "img/post-bg-kuaidi.jpg"
tags:
    - Linux
---

>看一个真正的专家操作命令行绝对是一种很好的体验-光标在单词之间来回穿梭，命令行不同的滚动。 
 在这里强烈建立适应`GUI`节目的开发者尝试一下在提示符下面工作。 
 但是事情也不是那么简单，还是需要知道“如何去做”。在单词之间跳转，使用`Ctrl+左右键`。

- 常用
```
Ctrl+左右键:在单词之间跳转
Ctrl+a跳到本行的行首
Ctrl+e则跳到页尾
Ctrl+u删除当前光标前面的文字
ctrl+k删除当前光标后面的文字
Ctrl+y粘贴Ctrl+u或Ctrl+k剪切的内容
Ctrl+L进行清屏操作
Ctrl+w删除光标前面的单词的字符
Alt+d删除光标后面的单词字符 
```

**1. 快速搜索已经输入过的命令**

&emsp;在执行命令时，我们经常用上下键去翻找最近执行过的命令，如果很久之前的命令，上下键就会力不从心，这时怎么办呢？

> - 1.1 方法一`Ctrl+r`快捷键(推荐)

&emsp;先输入`Ctrl+r`，输入要查找命令的关键词，会显示在中间部分第二个标记位置，如果找到相关命令，会显示到第三个标记位置，如果不是自己期望的命令，可以多次使用`Ctrl+r`翻找命令，然后按回车执行或者`->`键得到命令

    (reverse-i-search)`git commit -m ': git commit -m 'fix(.gitignore)'

> - 1.2 方法二`history`命令

```
history|grep '/home/work' 查找命令
!(id号) 执行命令
```



