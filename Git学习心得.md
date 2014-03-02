
#Git学习心得

#前言

本来今天是准备学习如何使用GitHub命令，按照[Git与Github入门资料](http://www.yangzhiping.com/tech/git.html)这篇教程操作了，出现很多问题，必须自己去搜索。而且按照这个操作后，还是不知道每个命令的意思。这篇教程太精简了，完全不适合新手入门。

- 没有说明SSH秘钥生成和安装

- 没有对文章中的命令进行解释。

完全看不懂他在说什么。所以还需要看其他的git的入门。

- [git-简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)这是一个个人博客，页面设计的很有感觉，但也不是面向普通小白的。先看之前的那篇文章，在看这篇，可能会理解一点吧。但个人感觉这两个教程，都是典型的国人教程。第一个人，直接罗列命令，不解释。第二个人，从很高的层次来解释命令，没有实例。

- [git入门](http://ryanflyer.iteye.com/blog/1664131)和[GitHub快速入门简单教程以及常用Git命令](http://blog.csdn.net/u012146107/article/details/12101069)，这两篇文章以类似于handbook的形式给出，比较容易懂。并且对每个命令都有解释。

推荐一下后者的教程。
但是现在发现了廖雪峰大神的个人博客，写的教程，通俗易懂。
看README.md中的介绍。
进入正文。
-----------

##建立仓库
本地建立仓库，就是找个目录作为代码存放地方。
所以在Msysgit中，cd到某个目录，mkdir建立一个存放代码的目录
比如：
> cd Document
> mkdir GitProject
> cd GitProject

进入到GitProject目录下后，使用git init命令对该目录进行初始化，
会生成.git文件，该文件就是一个记录文件提交的配置文件
命令:
> git init

##git add <file>
使用git add 添加文件，不论该文件是修改的，还是新添加的，都是采用git add <file>
##git status
可以查看是否有文件修改或者添加进来
##git diff <file>
可以查看该文件与已经提交过的文件的不同
其中
红色字体表示完全不同，并且会带有符号减
白色表示二者皆有，行前无符号
绿色表示新添加的，行前有加号
##git log
显示commit记录
##git log --pretty=oneline
以一行记录来显示commit记录，包括commit的版本号和-m后的消息，该版本号由SHA1计算出来。
##

