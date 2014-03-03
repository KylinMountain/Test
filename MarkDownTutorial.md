# 学习使用MarkDown在线编辑器
## Learn How to Use MarkDown Editor Online

------
我们理解您需要更高效更便捷的工具记录思想，整理笔记、知识，并将其中承载的价值传播给他们，*MartDown**是我们给出的答案————我们为记录思想和分享知识提供更专业的工具。

您可以使用**MarkDwon**:

- 整理知识，分享笔记
- 发布日记，杂文，所见所想
- 撰写发布技术文稿（代码支持）
- 撰写发布学术论文（LaTeX公式支持）

这是一份 Cmd Markdown 的欢迎稿兼使用说明，请保留，如需撰写**新稿件**，点击顶部工具栏的右侧的**新建文本**图标或者使用快捷键**Ctrl+Alt+N**

------
- 书写一个质能方程
>$E=mc^2$
- 或者高亮一段代码
```Python
def solution(a)
    n = len(a)
    sum = left = 0
    for i in range(0, n):
        sum += a[i]
    for i in range(0, n):
        if ( left = sum - a[i]- left):
            return i;
        left += a[i]
    return -1
```        
- 测试数据：
> a = [1,2,3,1,3,2,1]
- 结果为：
> 3

想要了解更详细的语法说明，可以参考我们准备的[MarkDown语法简明手册]

## 标题
这是最为常用的格式，在平时常用的的文本编辑器中大多是这样实现的：输入文本、选中文本、设置标题格式。

而在 Markdown 中，你只需要在文本前面加上#即可，同理、你还可以增加二级标题、三级标题、四级标题、五级标题和六级标题，总共六级，只需要增加  # 即可，标题字号相应降低。例如：
采用多个#来表示层级标题
```
# 一级标题
## 二级标题
### 三级标题
```
注：# 和「一级标题」之间建议保留一个字符的空格，这是最标准的 Markdown 写法。

## 列表

列表格式也很常用，在 Markdown 中，你只需要在文字前面加上 - 就可以了，例如：

- 文本1
- 文本2
- 文本3

如果你希望有序列表，也可以在文字前面加上 1. 2. 3. 就可以了，例如：

1. 文本1
2. 文本2
3. 文本3

##链接和图片
在 Markdown 中，插入链接不需要其他按钮，你只需要使用 [显示文本](链接地址) 这样的语法即可，例如：
[GitHub](https://github.com/)

在 Markdown 中，插入图片不需要其他按钮，你只需要使用 ![](图片链接地址) 这样的语法即可，例如：
![](http://ww4.sinaimg.cn/bmiddle/aa397b7fjw1dzplsgpdw5j.jpg)

## 引用
在我们写作的时候经常需要引用他人的文字，这个时候引用这个格式就很有必要了，在 Markdown 中，你只需要在你希望引用的文字前面加上 > 就好了，例如：
```
一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。
```
> 一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。

注：> 和文本之间要保留一个字符的空格。

## 粗体和斜体

Markdown 的粗体和斜体也非常简单，用两个 * 包含一段文本就是粗体的语法，用一个 * 包含一段文本就是斜体的语法。例如：
**粗体**
*斜体*
*一个段落一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。*

-----

#MarkDown学习心得

今天学习了MarkDown语法，觉得MarkDown显示效果非常简洁。之所以学习MarkDown，是一个偶然中带着必然的结果吧。原因有几下几点：

- MarkDown的作者Aaron Swartz的死，让我有幸了解到MarkDown

- GitHub的很多README文件都是以 md 文件来写的，简洁明了。

- 之前在SegmentFault上写过很费劲，今天了解了一下据说是混合了MarkDown和Wiki的语法

- 想锻炼自己的写作水平和表达能力

## 学习步骤

1. [**献给写作者的MarkDown指南**](http://jianshu.io/p/q81RER)，这是一篇MarkDown的简明教程，一学就会。

2. [**MarkDown的语法说明（简体中文）**](http://wowubuntu.com/markdown/)，官方MarkDown的中文说明，该文总以HTML的原码来解释MarkDown的语法，没有该MarkDown使用后，将产生何种样式的字体或者格式，太偏向于前段开发工程师。

3. [**StakcEdit**](https://stackedit.io/#)的开篇教程，StackEdit是一个MarkDown在线编辑器，只是教程英文的。事实上，SegmentFault上还有篇博文专门介绍了StackEdit，试用了一下功能确实很强大。

推荐在StackEdit中学习第一篇教程，可以帮助你很快的学习MarkDown的语法。

另外，在学习的过程中，还了解到一个叫做CMD-MarkDown的在线MarkDown的编辑器，但是我在StackEdit中练习CMD-MarkDown的教程，发现很多命令不相符，比如列表。



很多网站都不是采用标准的MarkDown，比如：

- GitHub

- StackEdit

都对SM进行了扩展。


------


> Written with [StackEdit](https://stackedit.io/).