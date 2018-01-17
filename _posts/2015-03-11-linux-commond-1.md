---
layout: post
title: 常用linux命令（1）--pwd、ls和cd
tags:
  - linux
---

### 一、pwd命令
`pwd`命令以绝对路径的方式显示用户当前工作目录。命令将当前目录的全路径名称（从根目录）写入标准输出。全部目录使用`/`分隔。第一个`/`表示根目录，最后一个目录是当前目录。执行`pwd`命令可立刻得知您目前所在的工作目录的绝对路径名称。
#### 1.示例
![pwd](http://7xtfpb.com1.z0.glb.clouddn.com/post/pwd.png)
### 二、ls命令
`ls`命令用来显示目标目录下的文件或者目标目录的信息，在Linux中是使用率最高的命令之一。
#### 1.语法

> ls [选项] [文件]

#### 2.常用选项

> `-a`: 显示指定目录下所有文件,包括以`.`开头的隐藏文件（linux中目录也是文件）
>
> `-A`: 显示`.`和`..`以外的所有文件，包括隐藏文件
>
> `-l`: 以长格式显示目录下的文件。输出信息有文件类型、权限、硬连接数、所有者组、文件大小和文件的最后修改时间，文件名等；
> 
> `-F`: 在每个输出项后追加文件的类型标识符，具体含义: `*`--可执行文件，`/`--目录，`@`--符号链接，`|`--管道，`=`--套接字，普通文件不输出标识符
>
> `-d`: 显示目录本身，而不显示目录下的内容
>
> `-i`: 显示文件索引节点号（inode）
>
> `-t`: 用文件和目录的更改时间排序
>
> `--full-time`: 列出完整的日期与时间

#### 3.示例

显示当前目录下的文件，不包括隐藏文件

    ls

![ls.1](http://7xtfpb.com1.z0.glb.clouddn.com/post/ls.1.PNG)
显示当前目录下包括隐藏文件在内的所有文件

    ls -a

![ls.2](http://7xtfpb.com1.z0.glb.clouddn.com/post/ls.2.PNG)
显示当前目录下文件的长格式信息

    ls -l

![ls.3](http://7xtfpb.com1.z0.glb.clouddn.com/post/ls.3.PNG)
显示某个文件的长格式信息，并显示节点号

    ls -li a

![ls.4](http://7xtfpb.com1.z0.glb.clouddn.com/post/ls.4.PNG)
显示某个目录的长格式信息

    ls -ld aaa

![ls.5](http://7xtfpb.com1.z0.glb.clouddn.com/post/ls.5.PNG)
在每个输出项后面加上类型标识符

    ls -aF

![ls.6](http://7xtfpb.com1.z0.glb.clouddn.com/post/ls.6.PNG)
### 三、cd命令
`cd`命令用来切换工作目录到目标目录。目标目录的表示法可以是绝对路径或相对路径。若目录名称省略，则变换至使用者的家目录。另外，`~`也表示家目录，`.`表示当前目录，`..`则表示当前目录的上一层目录。
#### 1.语法

> cd [选项] [参数]

#### 2.示例
切换至根目录

    cd /

![cd.1](http://7xtfpb.com1.z0.glb.clouddn.com/post/cd.1.PNG)
切换至家目录

    cd

![cd.2](http://7xtfpb.com1.z0.glb.clouddn.com/post/cd.2.PNG)
切换至之前停留的目录

    cd -

![cd.3](http://7xtfpb.com1.z0.glb.clouddn.com/post/cd.3.PNG)
切换至当前目录的上层目录

    cd ..

![cd.4](http://7xtfpb.com1.z0.glb.clouddn.com/post/cd.4.PNG)