---
title: hexo博客中添加categories分类
date: 2020-04-01 16:45:16
tags: hexo
categories: 学习
---

### 方法如下:

1. 在根目录下scaffolds/post.md中，添加一行 categories: 
    
        title: {{ title }}
        date: {{ date }}
        tags:
        categories:   //这行是新加的(这是注释) 

2. 实际编写文章的时候，在开头加上categories: 的标签。例如：

        ---
        title: Hello，World!你好，世界！
        date: 2014-01-21 23:33:02
        tags: java学习标签
        categories: 编程类
        ---
        
   这样在文章发布时，在git中使用hexo g命令，hexo会在根目录/public/categrises下自动生成归档文件夹
        
3. 用命令 hexo g -d 发布文章后会把文章自动添加到指定类别中

参考文章： [使用Hexo的内建归档categories](https://www.zhihu.com/tardis/landing/360/ans/58775540?query=hexo%E5%8D%9A%E5%AE%A2%E5%8F%AA%E8%83%BD%E5%9C%A8_post%E6%96%87%E4%BB%B6%E5%A4%B9%E5%86%99%E5%90%97&mid=c1f53aa2273cc629d1dd457d469e3c44&guid=FCC08D1993A3F1A3840F515E6C8B3D9B.1585216830677)