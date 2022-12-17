---
title: 蔡鸿凯的期末大作业
---
笔记:
1、linux环境下的基本操作命令，包括文件操作命令（rm mkdir chmod，chown）编辑工具使用(vi vim)linux用户管理（useradd userdel usermod）

2、linux的各种配置（环境变量配置，网络配置，服务配置）

3、linux下如何搭建对应语言的开发环境（大数据,JavaEE,Python）

4、能编写shell脚本，对Linux服务器进行维护

5、能进行安全设置，防止攻击，保障服务器正常运行，能对系统调优

6、深入理解Linux系统（对内核有研究）。熟练掌握大型网站应用架构组成、并熟悉各个环节的部署和维护方法

vi和vim的基本介绍
        所有的Linux系统都会内建vi文本编辑器
        Vim具有程序编辑的能力，可以看做是Vi的增强版本，可以主动地以字体颜色辨别语法的正确性，方便程序设计。代码补完、编译及错误跳转等方便编程的功能特别丰富。
![baidu logo](https://img-blog.csdnimg.cn/b8cc161d81c84230812c71cdb3eb889e.png)

添加用户
        语法：useradd [选项]  用户名
        添加一个  用户xm
![baidu logo](https://img-blog.csdnimg.cn/330f3801b97d4f698bc567af04a6ae0d.png)
		  特别说明：cd     表示change directory 切换目录
        当创建用户成功后，会自动的创建和用户同名的家目录
        也可以通过useradd -d 指定目录 新的用户名  ，给新创建的用户指定家目录
![baidu logo](https://img-blog.csdnimg.cn/abc8a12645a443c59eadbb3c9ce7eba2.png)

大作业完成步骤:
1.安装nodejs:生成静态页面
``` bash
$ sudo apt-get install nodejs
```
用nodejs -v 检查版本看是否安装上
2.安装npm：一会用来安装hexo
``` bash
$ sudo apt-get insall npm
```
3.正式安装hexo
``` bash
$ sudo npm install -g hexo
```
4.预备工作搞定，为了方便处理先建立一个hexo的文件夹
``` bash
$ mkdir hexo
$ cd hexo
```
5.建立自己的博客 hexo init chk
``` bash
$ cd chk
```
6.然后装个npm进去
``` bash
$ npm install
```
7.在博客目录下输入以下命令时，会默认使用post布局，然后自动在source\_posts目录生成一个homework.md文件：
``` bash
$ hexo new homework
```
