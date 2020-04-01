---
title: 如何上传本地文件到Github的repositories中
date: 2020-04-01 19：56
tags: Github
categories: 学习
---

# 如何上传本地文件到 Github 的repositories（仓库）中

### 第一种方法：
直接登入到Github网页，在线上传文件夹。
1. 可以直接拖拽上传整个文件夹
2. 也可以choose your files 上传单个文件。
<p> </p>
<p> </p>
<p> </p>

### 第二种方法：通过 git 工具在命令行中上传本地文件夹（本地项目）

1. 下载git工具：到([git官网（嘿！我是官网链接）](https://git-scm.com/))上下载

2. 绑定自己的电脑用户：
      1. 打开git-bash.exe，在命令行中输入：
    
        git config --global user.name "这里输入你的github注册账号"
        git config --global user.email "这里输入你的注册邮箱"
      2. 设置ssh key([git中的ssh key有什么用？(点击访问)](https://segmentfault.com/q/1010000000118744))
            1. 在电脑C盘生成ssh key 
            
                    ssh-keygen -t rsa -C "注册GitHub的邮箱号"
                    
            2. 生成过后，去对应目录C：\Users\.ssh里，用记事本打开 id_rsa.pub文件，复制里面的ssh key公钥
            3. 为Github账号配置ssh key:切换到github，展开个人头像的小三角，点击settings，然后打开SSH keys菜单， 点击New SSH key新增密钥，填上标题（最好跟本地仓库保持一致）。接着将id_rsa.pub文件中key粘贴到此，最后Add key生成密钥吧。
      
3. 新建一个Github仓库后，将这个本地文件夹关联新建的github仓库：

            git remote add origin 你的仓库地址     // 这样就把这个文件夹和指定仓库关联起来了

4.  把远端仓库的README.md 文件传到本地的文件夹中：

            git pull origin master     //这个命令行可以从远端取文件到本地中
    如果README.md 出现在本地文件夹中，则证明连接成功
    
5.  选一个想上传的本地文件夹,首先要把文件（或文件夹）上传到缓冲区,再从缓冲区到文件区，最后从文件区到GitHub仓库:

            git add 本地文件的完整文件名             // 添加文件到缓冲区
            /* git add .  //添加此文件夹的所有文件到缓冲区   */
            
            git commit -m "这里写对文件的描述,方便以后通过描述寻找文件"      // 双引号内是注释，这样就把文件从缓冲区提交到了文件区中

            git push origin master            // 这步是把文件区的内容上传到Github仓库中！
            
            
           
#### 欧克欧克、完成完成
