---
title: Lw‘s  First  Blog ——关于markdown语法
date: 2020-03-28
tags: markdown
categories: 随笔

---

#  markdown 语法
**注意**：写博客要在G:\blog\blog1\source\_posts目录下创建md文件（我自己用IDEA编写），
每次写完一篇blog之后都要重新打开 git 部署到GitHub上，输入的git命令行如下:
<p> hexo g -d </p>

## 关于取标题
”#“的个数代表标题的级数.

## 关于段落

<p align="center"><font face="微软雅黑" color="red" size="8px">这是一个红色的段落</font></p>

可以用html的p标签语法: \<p align="left">\<font face= "微软雅黑" color="red" size="28px">段落内容,字体,颜色,和字号的修改都可以用html语法 \</font>\</p>

## 关于引用的样式
引用标记用 ”>“ 表示，">后面跟引用内容", 样子如下：

>泰戈尔说过:"有一个夜晚我烧毁了所有的记忆，从此我的梦就透明了；有一个早晨我扔掉了所有的昨天，从此我的脚步就轻盈了"
><p></p>
><p>——来自酷狗《告白の夜》评论</p>

## 关于写一个列表
无序列表语法用这个标记“ - ”： “ - 无序列表 ”

- 无序列表1
- 无序列表2

<p>有序列表语法用这些序号“ 1. 2. 3. ”： “ 1.有序列表① ”&nbsp “ 2.有序列表② ”</p>

1. 有序列表①
2. 有序列表②

## 关于创建超链接语法

#### 图片超链接
<p>格式： ! [ 图片描述 ] ( 括号里跟图片地址 )</p>
<p>比如下图的链接格式： ！[皮卡丘的图片]（https：//*********.jpg）</p>

![皮卡丘的图片](https://p1.ssl.qhimg.com/dr/270_500_/t01b2a945701805d7f1.jpg?size=997x1024)

#### 网页超链接
<p>格式： [链接描述]（链接地址）</p>
<p>比如下方百度链接的格式：[baidu](https//www.baidu.com) </p>

[baidu](https//www.baidu.com)

## 关于文字风格

**加粗**： \*\*加粗** <p></p>
*斜体*: \*斜体\*<p></p>

## <p>以上是目前自己学习了的markdown语法的总结</p>