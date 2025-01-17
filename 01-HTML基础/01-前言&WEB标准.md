![img](https://i.loli.net/2020/12/01/uXGNF6CHE9dpVQt.jpg)

```
该笔记由【不言谢】，重新整理发布。以供更好的学习交流。
笔记中的图片全部传入PicGo中，换端不会再影响阅读。
```

联系方式：

​	不言谢的网络学习日志： https://www.cnblogs.com/byx1024/

​	不言谢の日常：https://www.byx1024.top/

------



> 第01阶段.前端基础.认识WEB
# 基础班学习目标

目标：  能根据psd文件，用HTML+CSS 布局出符合W3C规范的网页。

网站首页

![img](https://i.loli.net/2020/12/01/ka31RTJlfCyPVoD.jpg)

列表页、详情页、登录页、 注册页等等。。。。



# 课程安排

![kec](https://i.loli.net/2020/12/01/gJAaFXzEfwCjt8u.png)

 就业班详情 参看： http://www.itcast.cn/course/web.shtml

# HTML 第一天目标

  能够写出基本的html页面（里面包含图片、链接、文字等网页元素标签）

![a](https://i.loli.net/2020/12/01/c61DOZzIQfeuXMh.png)

# 认识WEB

## 1. 认识网页

```
网页主要由文字、图像和超链接等元素构成。当然，除了这些元素，网页中还可以包含音频、视频以及Flash等。
```

![mi](https://i.loli.net/2020/12/01/Xm2Q5JUCwY1g47F.png)

**思考：** 

网页是如何形成的呢?


![web](https://i.loli.net/2020/12/01/FLVjGUqytgfa589.png)



### 总结

网页有图片、链接、文字等元素组成，我们后面的任务就是要把这部分网页元素用代码写出来。。。

## 2. 浏览器（显示代码）

```
浏览器是网页显示、运行的平台，常用的浏览器有IE、火狐（Firefox）、谷歌（Chrome）、Safari和Opera等。我们平时称为五大浏览器。
```

![b](https://i.loli.net/2020/12/01/U8EtPxmkscQqFCl.png)

可能你最熟悉的是 IE浏览器，但是。。。

![liulan](https://i.loli.net/2020/12/01/LOaxCYFogA2hvEI.jpg)

### 2.1 查看浏览器占有的市场份额

查看网站： <a href="http://tongji.baidu.com/data/browser" target="_blank">http://tongji.baidu.com/data/browser</a>

![count](https://i.loli.net/2020/12/01/n4yw69pLDfXae8Z.png)

 2008年，大名鼎鼎的互联网巨头Google公司发布了它的首款浏览器Chrome浏览器。   

 跟王思聪一样，没办法，生下来人家就是富二代官二代啊，后台太强，而且确实先天能力得天独厚。 

**pink老师 一句话说出他们:**

> 出自谷歌，唯我不败；一统江湖，千秋万代。 

### 2.2 常见浏览器内核（了解）

首先解释一下浏览器内核是什么东西。英文叫做：Rendering Engine，中文翻译很多，排版引擎、解释引擎、渲染引擎，现在流行称为浏览器内核.

```
负责读取网页内容，整理讯息，计算网页的显示方式并显示页面.
```
因为浏览器太多啦， 但是现在主要流行的就是下面几个：

| 浏览器  |      内核      | 备注                                                         |
| :------ | :------------: | :----------------------------------------------------------- |
| IE      |    Trident     | IE、猎豹安全、360极速浏览器、百度浏览器                      |
| firefox |     Gecko      | 可惜这几年已经没落了，打开速度慢、升级频繁、猪一样的队友flash、神一样的对手chrome。 |
| Safari  |     webkit     | 现在很多人错误地把 webkit 叫做 chrome内核（即使 chrome内核已经是 blink 了）。苹果感觉像被别人抢了媳妇，都哭晕再厕所里面了。 |
| chrome  | Chromium/Blink | 在 Chromium 项目中研发 Blink 渲染引擎（即浏览器核心），内置于 Chrome 浏览器之中。Blink 其实是 WebKit 的分支。大部分国产浏览器最新版都采用Blink内核。二次开发 |
| Opera   |     blink      | 现在跟随chrome用blink内核。                                  |

**拓展阅读：**
```
移动端的浏览器内核主要说的是系统内置浏览器的内核。

Android手机而言，使用率最高的就是Webkit内核，大部分国产浏览器宣称的自己的内核，基本上也是属于webkit二次开发。

iOS以及WP7平台上，由于系统原因，系统大部分自带浏览器内核，一般是Safari或者IE内核Trident的
```

## 3. Web标准（重点）

目标

* 记忆
  * 能说出网页 中 web 标准三层组成
* 理解
  * 能结合人来表述web标准三层

Web标准不是某一个标准，而是由W3C组织和其他标准化组织制定的一系列标准的集合。

W3C 万维网联盟是国际最著名的标准化组织。1994年成立后，至今已发布近百项相关万维网的标准，对万维网发展做出了杰出的贡献。

**w3c就类似于现实世界中的联合国。**

### 3.1 为什么要遵循WEB标准呢？

 通过以上浏览器不同内核不同，我们知道他们显示页面或者排版就有些许差异。

![bz](https://i.loli.net/2020/12/01/B8Mvk7IcERnSlNG.png)

### 3.2 Web 标准的好处

遵循web标准可以让不同我们写的页面更标准更统一外，还有许多优点

*1*、让Web的发展前景更广阔 
*2*、内容能被更广泛的设备访问
*3*、更容易被搜寻引擎搜索
*4*、降低网站流量费用
*5*、使网站更易于维护
*6*、提高页面浏览速度

###  3.3 Web 标准构成

**构成：** 主要包括结构（Structure）、表现（Presentation）和行为（Behavior）三个方面。

| 标准 | 说明                                                         | 备注                                                         |
| :--- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| 结构 | 结构用于对**网页元素**进行整理和分类，咱们主要学的是HTML。   | ![htmll](https://i.loli.net/2020/12/01/2XrO8TjlZkadwnW.jpg)  |
| 表现 | 表现用于设置网页元素的版式、颜色、大小等**外观样式**，主要指的是CSS | ![css](F:\√学习课程\web前端黑马19年课程\【27】源码+课件+软件\01-03 前端开发基础\01-HTML资料\01.HTML-Day01\笔记\media\css.jpg) |
| 行为 | 行为是指网页模型的定义及**交互**的编写，咱们主要学的是 Javascript | ![search](F:\√学习课程\web前端黑马19年课程\【27】源码+课件+软件\01-03 前端开发基础\01-HTML资料\01.HTML-Day01\笔记\media\search.gif) |

 理想状态我们的源码： .HTML      .css      .js 



**结合人来记忆web标准：**

* 结构标准：   ![hb1](https://i.loli.net/2020/12/01/xworaNBnmWLdHeZ.png)是你天然的身体 





* 表现标准：   ![hb2](https://i.loli.net/2020/12/01/gnaSxjTycRGpIUk.png)  决定你是否打扮的美丽外观(衣服？化妆？)





* 行为标准：   ![hb3](https://i.loli.net/2020/12/01/YhCKTI4oSOkdLgF.gif)  决定你是否有吸引人的行为(动作)

****

### web标准小结

* web标准有三层结构，分别是结构（html）、表现（css）和行为（javascript）  
* 结构类似人的身体， 表现类似人的着装， 行为类似人的行为动作
* 理想状态下，他们三层都是独立的， 放到不同的文件里面

## 4. 拓展@

* **介绍一下你对浏览器内核的理解？常见的浏览器内核有哪些？**

  浏览器内核包括两部分，渲染引擎和js引擎。渲染引擎负责读取网页内容，整理讯息，计算网页的显示方式并显示页面，js引擎是解析执行js获取网页的动态效果。 后来 JS 引擎越来越独立，内核就倾向于只指渲染引擎。
  IE：Trident 
  firefox：Gecko 
  chrom、safari：webkit 
  Opera：Presto 
  Microsoft Edge：EdgeHTML

  深度阅读：[五大主流浏览器内核的源起以及国内各大浏览器内核总结](http://blog.csdn.net/summer_15/article/details/71249203) 