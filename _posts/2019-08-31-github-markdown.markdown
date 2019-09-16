---
title: "GitHub之Markdown语法"
layout: post
date: 2016-02-24 22:44
image: /assets/images/markdown.jpg
headerImage: false
tag:
- markdown
- elements
star: true
category: blog
author: johndoe
description: Markdown summary with different options
---

> Markdown是一种轻量级标记语言，创始人为约翰·格鲁伯（英语：John Gruber）。它允许人们“使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML（或者HTML）文档”。


## head

```
# Markdown
## Markdown
### Markdown
#### Markdown
##### Markdown
###### Markdown
```

以上对应内容对应如下：

# Markdown
## Markdown
### Markdown
#### Markdown
##### Markdown
###### Markdown

最多可以支持6个，而且需要注意的是，这里的#开头的文字或标题必须另起一行，#和文字中间必须有空格，不然GitHub的README无法识别。

## 段落和换行

- **分割线**

	---

分割线一般由---三个连续符合表示，单行开头，至少为三个。

- **换行**

换行可以使用一个或者多个空行来另起一个段落，注意是一个空行，而不是简单地用回车来另换一行，示例：

	第一行
	
	第二行
	第三行

如下所示，以空行代替换行。

第一行

第二行
第三行

- **插入文本引用**

```
正文

    引用文本
```

所对应的内容如下：

正文

	引用文本

- **列表**

**无序列表**

无序列表k而已使用* + -来标识，注意在字符之后要添加一个空格，示例：

	* markdown
	+ markdown
	- markdwon

对应显示内容如下：

- markdown

- **代码**

	`print "hello world"`

对应显示：

`print "hello world"`


- **链接**

添加链接：

[厉害了喵的博客](walkmao.top)

- **插入图片**

		![pic](https://raw.githubusercontent.com/linux-downey/bloc_test/master/picture/Makedown/Makedown.png)

> ![pic](https://raw.githubusercontent.com/linux-downey/bloc_test/master/picture/Makedown/Makedown.png)

- **修改图片大小**

如果要修改图片大小，可以使用HTML的处理方式来插入图片，并设置固定大小

```HTML
<img src="https://raw.githubusercontent.com/linux-downey/bloc_test/master/picture/Makedown/Makedown.png" width="%50" height="%50" />
```

- **插入表格**

表头 | 表头 | 表头
----| ---- | ----
cat | count | price
dog | 5 | 12.4

第二行分割表头和内容。 '-'有一个就行，为了对齐，多加了几个。文字默认居左，两边加‘-’：表示文字居中；右边加‘-’：表示文字居右。