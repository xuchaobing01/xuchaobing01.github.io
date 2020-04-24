---
layout:       post
title:        "Markdown 基础使用"
subtitle:     "Markdown的基础使用语法，如何去使用Markdown"
date:         2018-06-16 12:00:00
author:       "Sean"
header-img:   "img/in-post/post-eleme-pwa/eleme-at-io.jpg"
header-mask:  0.3
catalog:      true
multilingual: false
tags:
    - Markdown
---

## 前言

Markdown是一种轻量级的**标记语言**，文本编辑器，被广泛运用于写作上，规范文本格式。类似的编辑器还有百度[UEditor](http://ueditor.baidu.com/website/onlinedemo.html) .

<!--[Markdown【基础篇】地址：](https://worktile.com/blog/skills/markdown)-->

## 1. 标题(共六级标题，一般也就用到三级)

```
# h1 一级标题
## h2 二级标题
### h3 三级标题
#### h4 四级标题
##### h5 五级标题
######  h6 六级标题
```

效果：

# h1 一级标题
## h2 二级标题
### h3 三级标题
#### h4 四级标题
##### h5 五级标题
######  h6 六级标题

## 2. 链接（有两种写法)

第一种 `[text](url)`:

```
语法：[text](url)
例子：[百度](http://www.baidu.com "百度"){:target="_blank"}
```

第二种 `[text][id] [id]:url`:

```
语法：
[text][id]
[id]:url
例子：
[百度][1]
[淘宝][2]
...
[1]:http://www.baidu.com '百度'
[2]:http://www.taobao.com '淘宝'
...
```

效果：

[百度][1]
[淘宝][2]

[1]:http://www.baidu.com '百度'
[2]:http://www.taobao.com '淘宝'

## 3. 图片

```
语法：![](image-url)
例子：![](https://raw.githubusercontent.com/xuchaobing01/xuchaobing01.github.io/master/img/post-markdown.jpg)
```

效果：

![](https://raw.githubusercontent.com/xuchaobing01/xuchaobing01.github.io/master/img/post-markdown.jpg)

## 4.加粗`**文字**`

```
语法：**文字**
例子：这本书的名字叫**这是你要加粗的内容**
```

效果：

这本书的名字叫**这是你要加粗的内容**

## 5.斜体 `*文字*`

```
语法：**文字**
例子：你是多*这是你要加斜的内容*
```

效果：

你是多*这是你要加斜的内容*

## 6. 代码与代码块


    `代码`
    或
    ```
    function index(){
        $article=Article::latest()->get();
        reutnr view('aritlce.index',compact('article'));
    }
    ```

效果：

执行`php artisan migrate`命令

```
function index(){
    $article=Article::latest()->get();
    reutnr view('aritlce.index',compact('article'));
}
```

# 7.无序列表 #

```
* 无序列表1
* 无序列表2
* 无序列表3
* 无序列表4
一个星号加一个空格，注意星号与文字之间有一个空格
```

效果：

* 无序列表1
* 无序列表2
* 无序列表3
* 无序列表4

# 8.有序列表 #

```
1. 有序列表1
2. 有序列表2
3. 有序列表3
4. 有序列表4
一个数字加一个点，文子与点之间有一个空格
```

效果：

1. 有序列表1
2. 有序列表2
3. 有序列表3
4. 有序列表4

## 9. 引用 `>` 

```
> 这是引用的内容
> 引用内容二
> 向右的尖括号表示引用
```

效果：

>这是引用的内容
>
> 引用内容二
>
> 向右的尖括号表示引用

## 10. 分割线 `***` 

```
***
用连续的三个星号表示
----------
```

效果：

***

用连续的三个星号表示

----------

## 11. 空格 `&ensp; &emsp;`

```
&ensp;一个空格`&ensp; `
&emsp;两个空格，常用于段落缩进`&emsp;`
```

效果：

&ensp;一个空格`&ensp; `

&emsp;两个空格，常用于段落缩进`&emsp;`

## 12. 表格

语法：


    | uid | name | password | email |
    |----|:-----:|:--------:|------:|
    | 1 | 张三 | 123456 | zhangsang@qq.com |
    | 2 | 李四 | eofj343hf | lisi@163.com |
    | 3 | 王二 | DoFj3D#43hf | wang@163.com |


效果：

|  uid  |  name  |  password  |      email        |
|-------|:------:|:----------:|------------------:|
| 1     | 张三   | 123456     | zhangsang@qq.com  |
| 2     | 李四   | eofj343hf  | lisi@163.com      |
| 3     | 王二   | DoFj3D#43hf | wang@163.com     |


## 13. 目录文件结构

    bootstrap/
    └── dist/
        ├── css/
        │   ├── bootstrap-grid.css
        │   ├── bootstrap-grid.css.map
        │   ├── bootstrap-grid.min.css
        │   ├── bootstrap-grid.min.css.map
        │   ├── bootstrap-reboot.css
        │   ├── bootstrap-reboot.css.map
        │   ├── bootstrap-reboot.min.css
        │   ├── bootstrap-reboot.min.css.map
        │   ├── bootstrap-utilities.css
        │   ├── bootstrap-utilities.css.map
        │   ├── bootstrap-utilities.min.css
        │   ├── bootstrap-utilities.min.css.map
        │   ├── bootstrap.css
        │   ├── bootstrap.css.map
        │   ├── bootstrap.min.css
        │   └── bootstrap.min.css.map
        └── js/
            ├── bootstrap.bundle.js
            ├── bootstrap.bundle.js.map
            ├── bootstrap.bundle.min.js
            ├── bootstrap.bundle.min.js.map
            ├── bootstrap.esm.js
            ├── bootstrap.esm.js.map
            ├── bootstrap.esm.min.js
            ├── bootstrap.esm.min.js.map
            ├── bootstrap.js
            ├── bootstrap.js.map
            ├── bootstrap.min.js
            └── bootstrap.min.js.map

