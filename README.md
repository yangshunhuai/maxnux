# PELinux
以Linux为内核的系统维护工具。

## 介绍
多数电脑问题WinPE都是可以解决的，但是在某些情况下不行。

比如说，当电脑的分区表产生了损坏的时候，Windows是无法启动的。在这种情况下，就需要Linux的帮助来修复问题。

PELinux是一个基于Linux的维护系统，内置有fdisk、gdisk等Unix下著名的分区工具和各种其他工具，可以修复很多电脑问题。

## 构建方法
1. 将完整系统打包。

   现在并不打算使用这个方法，因为无论如何精简也无法把系统做到50MB以内。
2. 取出完整系统中的内核和初始化内存盘，手动移植所有程序。

   这个方法是可行的，目前先打算用这个方法试一下，将来再用手动编译法。
3. 从内核起，所有程序都手动编译，组合在一起。

   这是将来打算使用的方法。该种方法可定制性超强，最小的系统可以做到磁盘占用8MB以内还能运行Apache服务器。

   [Linux From Scratch](https://linuxfromscratch.org)是一个很好的主意。
