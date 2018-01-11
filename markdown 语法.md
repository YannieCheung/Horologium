---
title: markdown 语法 
tags: 新建,模板,小书匠
grammar_cjkRuby: true
---
<span id='top'></span>
# 目录
[toc]
# 常用语法

___

## 标题

#这是 H1 一级标题
##这是 H2 二级标题

## 列表
### 无序列表
* 项目1
  * 子项目1.1
  * 子项目1.2
    * 子项目1.2.1
* 项目2

+ 项目1
  + 子项目1.1
  + 子项目1.2
    + 子项目1.2.1
+ 项目2

- 项目1
  - 子项目1.1
  - 子项目1.2
    - 子项目1.2.1
- 项目2

### 有序列表
1. 项目1
2. 项目2
3. 项目3
    1. 项目3.1
    2. 项目3.2

1. 项目1
1. 项目2
1. 项目3
    1. 项目3.1
    1. 项目3.2

### 有序列表起始编号
58. 项目5
2. 项目6

## 链接
[返回顶部](#top)
[README](./README,md)
[README][adr]

[adr]: ./README.md        "Google" 

## 图片
![node.js](https://www.linuxfoundation.org/wp-content/uploads/2017/05/nodejs_logo.png)
![node.js][1]

[1]: https://www.linuxfoundation.org/wp-content/uploads/2017/05/nodejs_logo.png "node"

## 文字格式
**这是文字粗体格式**
__这是文字粗体格式__
*这是文字斜体格式*
_这是文字斜体格式_
~~在文字上添加删除线~~

## 引用
> 第一行引用文字
> 第二行引用文字

## 水平线
***


# GFM扩展语法
## 表格
First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

## 代码
### 行内代码
`var x = "hello world"`

### 块代码
```javascript
var a = "hello world";
var b = "good luck";
```

## 自动转换成超链接
https://github.com/

## HTML
<div class="hey">Hello world</div>

## 扩展的文字格式
++插入的文字++
==被记号的文字==
上角文字: 19^th^
下角文字: H~2~O

## 印刷字替换
系统将自动替换下列文字，转换成排版系统使用的符号
(c) (C) (r) (R) (tm) (TM) (p) (P) +-

## 缩写定义
The HTML specification
is maintained by the W3C.
*[HTML]: Hyper Text Markup Language
*[W3C]:  World Wide Web Consortium

## 待办事项
-[ ] 未完成事项
-[ ] 未完成事项
-[x] 完成事项
-[X] 完成事项

## 脚注
脚注[^1x]
[^1x]: 脚注的用法

## 定义
苹果
: 一种水果
: 一种品牌，计算机，手持设备
桔子
: 一种水果

## 公式

### 行内公式
这是行内公式`!$ \Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,. $`

### 块公式
```mathjax!
$$\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.$$
```

### 流程图 ([语法](http://adrai.github.io/flowchart.js/))
```flow
st=>start: 开始
e=>end: 结束
op=>operation: 操作步骤
cond=>condition: 是 或者 否?

st->op->cond
cond(yes)->e
cond(no)->op
```

```sequence
小明->小李: 你好 小李, 最近怎么样?
Note right of 小李: 小李想了想
小李-->小明: 还是老样子
```
