---
title: Hello World
tags:
	- hexo搭建
categories: 
	- hexo搭建
---
本站基于[Hexo](https://hexo.io/)!总算把blog网站搞好了，<!-- more -->其实很久以前就要高了，但是懒！！！所以一直没搞，今天算是把该搞的都高了一下，以后就开始慢慢写文章吧~~！

## 快速启动

### 创建新文章

``` bash
$ hexo new "My New Post"
```
创建的文章去根目录的source目录的_posts下去找对应的文件，然后可以在头部加入对应的标签和分类
如：
``` bash
tags: - hexo搭建
categories: hexo搭建
```
这样可以增加分类和标签以后就可以找对应的标签去文章，还有hexo所有的属性名称后面的`:都要加空格，不然报错！
详情: [Writing](https://hexo.io/docs/writing.html)

### 本地启动

``` bash
$ hexo server
```

详情: [Server](https://hexo.io/docs/server.html)

### 生成静态文件

``` bash
$ hexo clean 
$ hexo generate
```

详情： [Generating](https://hexo.io/docs/generating.html)

### 部署网站

``` bash
$ hexo deploy
```

详情: [Deployment](https://hexo.io/docs/deployment.html)

参考文档：[Hexo官网](https://hexo.io/)
		  [Next主题使用](http://theme-next.iissnan.com/getting-started.html)
		  [这个很全很详细感谢楼主](http://www.jianshu.com/p/5fc4672b7d2e)
