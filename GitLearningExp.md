
#Git学习心得

#前言

本来今天是准备学习如何使用GitHub命令，按照[Git与Github入门资料](http://www.yangzhiping.com/tech/git.html)这篇教程操作了，出现很多问题，必须自己去搜索。而且按照这个操作后，还是不知道每个命令的意思。这篇教程太精简了，完全不适合新手入门。

- 没有说明SSH秘钥生成和安装

- 没有对文章中的命令进行解释。

完全看不懂他在说什么。所以还需要看其他的git的入门。

- [git-简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)这是一个个人博客，页面设计的很有感觉，但也不是面向普通小白的。先看之前的那篇文章，在看这篇，可能会理解一点吧。但个人感觉这两个教程，都是典型的国人教程。第一个人，直接罗列命令，不解释。第二个人，从很高的层次来解释命令，没有实例。

- [git入门](http://ryanflyer.iteye.com/blog/1664131)和[GitHub快速入门简单教程以及常用Git命令](http://blog.csdn.net/u012146107/article/details/12101069)，这两篇文章以类似于handbook的形式给出，比较容易懂。并且对每个命令都有解释。

但是现在发现了廖雪峰大神的个人博客，写的教程，通俗易懂。
看README.md中的介绍。本篇文档是根据对该教程的学习时写的笔记或者摘要，比较粗糙。

好了，废话不多说进入正文。
-----------

##建立仓库
本地建立仓库，就是找个目录作为代码存放地方。
所以在Msysgit中，cd到某个目录，mkdir建立一个存放代码的目录，并进入该目录
比如：
> cd Document
> mkdir GitProject
> cd GitProject

进入到GitProject目录下后，使用git init命令对该目录进行初始化，
会生成.git文件，该文件Git的版本库
命令:
> git init

##git add <file>
使用git add 添加文件，不论该文件是修改的，还是新添加的，都是采用git add <file>
##git status
可以查看是否有文件修改或者添加进来
##git diff <file>
可以查看该文件与已经提交过的文件的不同。
其中（还不确定），
- 红色字体表示完全不同，并且会带有符号减
- 白色表示二者皆有，行前无符号
- 绿色表示新添加的，行前有加号

##git log
显示commit记录

##git log --pretty=oneline
以一行记录来显示commit记录，包括commit的版本号和-m后的消息，该版本号由SHA1计算出来。

##git reset --hard HEAD^
用于回退到某个commit，其中HEAD^表示回退到上一个提交版本
HEAD^^表示回退到上上个版本，HEAD~100表示回退到100个提交版本之前
这就好比穿越时光机
此时，在用git log就不会出现该版本之后的版本了
但只要该命令行窗口未关闭，你可以查看之前使用git log显示的版本号前几位
比如0a33aaa,无需全部的版本号，前几位即可。

## git reflog
该命令即是为了在关闭命令行窗口后，如何寻找之前的命令记录
该命令会显示所有的commit 记录。

##小结

HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id。

穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。

要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。

## 工作区和暂存区
分为工作区和版本库，其中版本库包括一个暂存区Stage和一个Master，HEAD指针指向Mater。
工作区，是还未进行add和commit的文件，此时的通过git status查看，这样的文件是untracked的。

当执行add时，将工作区的文件add到Stage中，接着使用commit就会将stage区中的文件提交到Master分支中。
关系如下图所示。

![](http://www.liaoxuefeng.com/files/attachments/001384907720458e56751df1c474485b697575073c40ae9000/0)

暂存区是很重要的概念。

##管理修改
为什么Git比其他版本控制系统设计得优秀，因为Git跟踪并管理的是修改，而非文件。






