---
title:  Add New Article
date: 2023-10-15 15:57:00
categories:
- Tools
tags:
- Tools
order: 1
---

# 如何添加新的文档

## 事前准备

### 登录github
打开[github](https://github.com)主页，输入账号密码登录，进入github个人主页，如下图所示。  
![github-main-page](https://github.com/limited-capacity/limited-capacity.github.io/raw/master/pictures/github-main-page.png)  
红框中的项目就是个人网页的主要代码。

### 代码结构
进入项目中，可以看到下面的代码目录结构  
![code-structure](https://github.com/limited-capacity/limited-capacity.github.io/raw/master/pictures/code-structure.png)  
第一个红框 `_posts` 是放置文章的文件夹，新建文档的话，需要在这个文件夹里新建。  
第二个红框 `pictures` 是放置图片的文件夹，如果文章中需要嵌入一些图片，可以将图片放置在这个文件夹内。

## 如何编辑
这里提供两个编辑方式。

#### 在线编辑
这种方式是比较方便的，但是功能不是很全，不过不需要使用额外的编辑器，如果只是做一些文字编辑，完全没有问题，新人友好。  
  
只需要在代码目录界面，点击键盘上的 `.` ，即可进入，没错，就是句号键。如下图所示。  
![github-ide](https://github.com/limited-capacity/limited-capacity.github.io/raw/master/pictures/github-ide.png)  
这里看似很复杂，但是需要关心的只有三块。  
第一块，左侧目录区。在这里可以看到项目中有哪些文件，以及想要添加新的文件时，可以在这个区域进行添加。在某个目录上，右键之后，会弹出一个弹框，可以进行一些操作。  
第二块，右侧编辑区。在左侧点击某个文件后，可以在这个区域对文件进行编辑，编辑主要是用 `markdown` 语法。不会的话可以看下这个文档[markdown](http://xianbai.me/learn-md/index.html)。编辑完成后需要进行`command + s`保存。  
第三块，最左侧一排按钮的第三个，点击后就是提交改动的区域，如果想要提交改动，需要有几个操作，如下图所示。  
![git-area](https://github.com/limited-capacity/limited-capacity.github.io/raw/master/pictures/git-area.png)  
- 第一步，需要将修改的内容保存
- 第二步，点击图片中的第一步的加号，将修改的内容加入缓存区
- 第三步，在上面的输入框中，输入这次改动的内容，如新建文档等
- 第四步，点击 `Commit & Push` 按钮，即可提交内容。
- 第五步，过一两分钟，刷新主页，恭喜你，能看到提交的文档了。

#### IDE编辑
IDE是指编辑器，可以使用vscode，使用方式和上述的方式一致，估计你也不会用，不介绍了。;-)

## 文章格式
除了上面讲到的需要用markdown语法进行编辑之外，新建的文档需要遵循以下的格式要求：
- 文件名格式：`年份数字-月份数字（两位）-日期数字（两位）-文章标题.md`
- 文件内容需要是下面的内容为开头  
![article-header](https://github.com/limited-capacity/limited-capacity.github.io/raw/master/pictures/article-header.png)

## 插入图片
在文章中插入图片应该是刚需，所以这里说一下。将你要插入的图片下载到本地，然后拖动到 `pictures` 这个文件夹中，就可以在文档中引用了，引用方式如下。
- 使用图片引入语法，即 `![]()` ,中括号内的是图片的名称，小括号内的是图片的地址，由于我们已经把图片放入 `pictures` 文件夹中了，所以我们可以用如下方式引用，`![git-area](https://github.com/limited-capacity/limited-capacity.github.io/raw/master/pictures/git-area.png)  ` 其中 `git-area` 是图片名称，后面的链接是地址，链接可以统一使用 `https://github.com/limited-capacity/limited-capacity.github.io/raw/master/pictures/` + 图片名称 + 后缀 的方式。