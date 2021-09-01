---
title: HTML学习笔记
tags: HTML
declare: true
abbrlink: 34391
date: 2020-10-18 11:08:00
---

# HTML学习笔记

## HTML简介

超文本标记语言（英语：HyperText Markup Language，简称：HTML）是一种用于创建网页的标准标记语言。html使用标记标签来描述网页，标签是用尖括号包围的关键词<>，且总是成对出现，例<font color= 'red'> <html>      </html> </font>其中<html>称为开始标签，</html>称为结束标签。HTML文档=网页，包含HTML标签和纯文本。

<!--more-->

html文件后缀  .html/.htm 都可以使用，没有区别

<font color='red'>**注意：**对于中文网页需要使用 **<meta charset="utf-8">** 声明编码，否则会出现乱码。有些浏览器(如 360 浏览器)会设置 GBK 为默认编码，则你需要设置为**<meta charset="gbk">。**</font>

参考W3school：

[HTML实例](https://www.w3school.com.cn/example/html_examples.asp)

[HTML参考手册](https://www.w3school.com.cn/tags/index.asp)

可以学习html的网站：

- [W3school](https://www.w3school.com.cn/)

- [菜鸟教程](https://www.runoob.com/html/html-tutorial.html)

- [freecodecamp(html练习)](https://www.freecodecamp.one/)

  

  

## HTML编辑器

编写html文件的编辑器有很多，可以使用Notepad或者TextEdit，sublime来编写HTML，文本编辑器同样可以编写html文件，如简单的txt文本编辑器，Typora文本编辑器。同样有专业编写HTML的编辑器。

- Adobe Dreamweaver
- Microsoft Expression Web
- CoffeeCup HTML Editor

## HTML元素

**注：为保证显示，所有标签前后都加了空格。**

### HTML元素语法

html元素指开始标签到结束标签的所有代码。

语法：

- 以开始标签开始

- 以结束标签结束

- html元素的内容指开始标签到结束标签之间的内容

- 某些html元素具有空内容

- 空元素在开始标签中进行关闭

- html元素可拥有属性

  

### HTML元素嵌套

多数html元素可以嵌套其他的html元素

例：

```
<html>

<body>
<p>html学习笔记</p>
</body>

</html>
```

其中< body >和< p >便嵌套在< html >元素中

### 空的HTML元素

没有内容的HTML元素被称为空元素。空元素在开始标签中被关闭。**< br >**（定义换行）就是没有结束标签的html空元素。**< br >**在所有浏览器中都有效，长远起见建议使用**< br/ >**

## HTML属性

html中的属性是为元素提供附加信息。属性以名称/值对的形式出现。例如：name="value"。属性总在开始标签中定义。

属性值始终被包括在尖括号中，且属性值应该被加以引号，双括号和单引号都可以，但双引号是最常见的。

<font color=red>*注意：当属性值本身带有双引号时，对属性值使用单引号*</font>

[HTML标准属性参考手册](https://www.w3school.com.cn/tags/index.asp)

属性实例

```
<a href="http://www.w3school.com.cn">This is a link</a>
```



## HTML标题

在html中，标题(heading)通过标签<font color="red">< h1 >-< h6 ></font>来进行定义

其中< h1 >定义最大的标题，< h6 >定义最小的标题

<font color="red">注意：浏览器会自动地在标题的前后添加空行</font>

### html水平线

<h r />标签用于在html页面中创建水平线

所以hr元素可以用于分隔内容

实例：

```
<p>This is a paragraph</p>
<hr />
<p>This is a paragraph</p>
<hr />
<p>This is a paragraph</p>
```

### html注释

注释的作用是提高代码可读性，可以更容易被人所理解，浏览器不会显示注释内容

html中使用<!--  注释  -->来编写注释

实例：

```
<!-- This is a comment -->
```

可以注释一行或一段代码

实例：

```
<!-- 此刻不显示图片：
<img border="0" src="/i/tulip_ballade.jpg" alt="Tulip">
-->
```



## HTML段落

html中通过<p>标签定义段落，这样可以把html段落划分为若干个段落，标签<p>有结束标签</p>,但是不写结束标签大多数浏览器也能正常的显示出来，为了形成好习惯，一般都会写上结束标签。

在html中会遇到空行问题，使用< p >< /p >能够产生空行，但是更建议使用上面说到的没有结束标签的html标签< br/ >

实例：

```
<p>This is a paragraph</p>
<p>This is another paragraph</p>
```



## HTML样式

html中style属性用于改变html元素的样式

实例：

```
<!--背景颜色:background-cloor-->
<html>

<body style="background-color:yellow">
<h2 style="background-color:red">This is a heading</h2>
<p style="background-color:green">This is a paragraph.</p>
</body>

</html>
```

```
<!--设置字体颜色和尺寸:font-family、color、font-size-->
<html>

<body>
<h1 style="font-family:verdana">A heading</h1>
<p style="font-family:arial;color:red;font-size:20px;">A paragraph.</p>
</body>

</html>
```

```
<!--文本对齐-->
<html>

<body>
<h1 style="text-align:center">This is a heading</h1>
<p>The heading above is aligned to the center of this page.</p>
</body>

</html>
```



## HTML文本格式化

html很多标签提供多种输出格式的标签

文本格式化标签：

| 标签       | 描述                                  |
| :--------- | :------------------------------------ |
| < b >      | 定义粗体文本。                        |
| < big >    | 定义大号字。                          |
| < em >     | 定义着重文字。                        |
| < i >      | 定义斜体字。                          |
| < samll >  | 定义小号字。                          |
| < strong > | 定义加重语气。                        |
| < sub >    | 定义下标字。                          |
| < sup >    | 定义上标字。                          |
| < ins >    | 定义插入字。                          |
| < del >    | 定义删除字。                          |
| < s >      | *不赞成使用。*使用 < del > 代替。     |
| < strike > | *不赞成使用。*使用 < del > 代替。     |
| < u >      | *不赞成使用。*使用样式（style）代替。 |

计算机输出标签：

| 标签          | 描述                              |
| :------------ | :-------------------------------- |
| < code >      | 定义计算机代码。                  |
| < kbd >       | 定义键盘码。                      |
| < samp >      | 定义计算机代码样本。              |
| < tt >        | 定义打字机代码。                  |
| < var >       | 定义变量。                        |
| < pre >       | 定义预格式文本。                  |
| < listing >   | *不赞成使用。*使用 < pre > 代替。 |
| < plaintext > | *不赞成使用。*使用 < pre > 代替。 |
| < xmp >       | *不赞成使用。*使用 < pre > 代替。 |

引用和术语定义：

| 标签           | 描述               |
| :------------- | :----------------- |
| < abbr >       | 定义缩写。         |
| < acronym >    | 定义首字母缩写。   |
| < address >    | 定义地址。         |
| < bdo >        | 定义文字方向。     |
| < blackquote > | 定义长的引用。     |
| < q >          | 定义短的引用语。   |
| < cite >       | 定义引用、引证。   |
| < dfn >        | 定义一个定义项目。 |



## HTML引用

在html文本格式化中有提到引用的标签

### < q >

< q >标签用于短的引用，浏览器会对< q >标签所所引用的内容加上引号

实例：

```
<p>WWF 的目标是：<q>构建人与自然和谐共存的世界。</q></p>
```

### < blockquote >

< blockquote >标签用于长引用，并且浏览器通常会对< blockquote >元素进行缩进处理

实例：

```
<p>以下内容引用自 WWF 的网站：</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
五十年来，WWF 一直致力于保护自然界的未来。
世界领先的环保组织，WWF 工作于 100 个国家，
并得到美国一百二十万会员及全球近五百万会员的支持。
</blockquote>
```

### < abbr >

< abbr >元素定义缩写或者首字母缩略语

对缩写进行标记能够为浏览器，翻译系统以及搜索引擎提供有用的信息

实例：

```
<p><abbr title="World Health Organization">WHO</abbr> 成立于 1948 年。</p>
```

### < dfn >

< dfn >元素定义项目或缩写的定义

1.如果< dfn >中设置了tittle属性，则定义项目：

```
<p><dfn title="World Health Organization">WHO</dfn> 成立于 1948 年。</p>
```

2.如果< dfn >元素包含具有标题的< abbr >元素，则tittle定义项目：

```
<p><dfn><abbr title="World Health Organization">WHO</abbr></dfn> 成立于 1948 年。</p>
```

3.如果什么都没有，则< dfn >文本内容即是项目，并且父元素包含定义：

```
<p><dfn>WHO</dfn> World Health Organization 成立于 1948 年。</p>
```

### < address >

< address >元素用于定义文档的作者或者文章的联系信息

此元素通常以斜体显示，多数浏览器会在此元素的前后添加空行

实例：

```
<address>
Written by Donald Duck.<br> 
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```

### < cite >

< cite >元素用于定义元素的标题

浏览器通常会以斜体显示< cite >元素

实例：

```
<p><cite>The Scream</cite> by Edward Munch. Painted in 1893.</p>
```

### < bdo >

< bdo >元素定义双向流覆盖，会覆盖当前文本方向，即从右向左进行书写

实例：

```
<bdo dir="rtl">This text will be written from right to left</bdo>
```



## HTML计算机代码元素

html具有专门显示计算机代码的标签，不需要使用属性去专门修改字母尺寸和字母间距

### < kbd >

< kbd >元素定义计算机输入

实例：

```
<p>To open a file, select:</p>

<p><kbd>File | Open...</kbd></p>

```

### < samp >

< samp >元素定义计算机输出示例：

实例：

```
<samp>
demo.example.com login: Apr 12 09:10:17
Linux 2.6.10-grsec+gg3+e+fhs6b+nfs+gr0501+++p3+c4a+gr2b-reslog-v6.189
</samp>
```

### < code >

< code >元素定义编程代码示例：

实例：

```
<code>
var person = { firstName:"Bill", lastName:"Gates", age:50, eyeColor:"blue" }
</code>
```

且< code >元素不会保留多余的空格和折行，即所有代码内容会在一行输出

实例：

```
<p>Coding Example:</p>

<code>
var person = {
    firstName:"Bill",
    lastName:"Gates",
    age:50,
    eyeColor:"blue"
}
</code>
```

如果想解决这一问题，可以使用< pre >元素包围代码

实例：

```
<p>Coding Example:</p>

<code>
<pre>
var person = {
    firstName:"Bill",
    lastName:"Gates",
    age:50,
    eyeColor:"blue"
}
</pre>
</code>
```

此时代码内容会存在空格和折行，而不是在一行输出

### < var >

< var >元素定义数学变量

可以进行数学公式的输出

实例：

```
<p>Einstein wrote:</p>

<p><var>E = m c<sup>2</sup></var></p>
```

