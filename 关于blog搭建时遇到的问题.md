---
title: 关于blog搭建时遇到的问题——fatal：unable to auto-detect email address
date: 2020-03-27
tags: 随笔
categories: 学习
---

自己动手搭建blog因为一个小问题花了小半天时间，错因：
fatal: unable to auto-detect email address

## 问题描述

用github和git搭建blog的时候,输入最后一步:
<p>npm install hexo-deloyer-git --save</p>
出错：fatal: unable to auto-detect email address

## 解决方法

参考网上的解决方法就是找到.deploy_git中的隐藏文件.git(显示隐藏文件的方法自行百度)，再找到.git目录中的config文件，在最后边加上三行(其实其他地方也存在.git文件，如果不确定就把全部.git后面都加上下面三行)：
 ``` bash
 [user]
 email=your email 
 name=your name
 ```
 
  <p><font color="red">注意[user]的括号要英文</font></p>