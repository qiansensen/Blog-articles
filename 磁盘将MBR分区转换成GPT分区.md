---
title: Windows无法安装到这个磁盘。选中的磁盘具有 MBR 分区表。在 EFI 系统上，Windows只能安装到GPT磁盘。
date: 2020-03-30
tags: 随笔
categories: 生活
---

![图片](https://picabstract-preview-ftn.weiyun.com/ftn_pic_abs_v3/f8e247eac94f0af34af3ac70e71a3ff40a3fb935f41380fad83a29af7fbdfd159d9a352e7b2a7e7beaec4e002bcb3780?pictype=scale&from=30113&version=3.3.3.3&uin=2609828363&fname=9EE84EABFBBF6F92FE59DE0E52F129FF.jpg&size=750)

### 下面是在 EFI系统上，将 MBR 磁盘转换成 GPT磁盘的方法

   1. Shift + F10 打开cmd窗口；
   2. 输入 Diskpart ，按下回车；
   3. 输入 list disk ， 列出磁盘列表，可以查看磁盘容量来判断需要转化格式的磁盘；
   4. 输入 select disk 0  ，看你select 哪个disk ，这里用 disk 0 举例；
   5. 输入 Clean ，清空磁盘，操作前确认磁盘中无重要文件；
   6. 输入 convert gpt ， 将MBR分区转换成GPT分区，反过来也行（convert mbr）;
   7. 拿下;