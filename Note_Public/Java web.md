> 平时60%
>
> ​	练习+测试20%
>
> 大作业40%(做网站+汇报  不超过3人)
>

> VScode 中F5运行
>

html写内容；css外观

b/s属于c/s

动态网站：更具用户请求动态生成页面信息

JDK  ec。。

meta 标记网页属性，单标记

## 网页语言

单标签也成为“空标签”

### 行标题

```html
h1....h6
h1{
	font-size:18px;
}
```



### 注释

```html
<!--内容-->
```

### 段落标签

```html
<p>
</p> //p 表示行号如h1、h2
```

### 行内标签

```html
<span>
</span>
```

### 换行标签

```html
<br/> 或 <br>
```

### 文本样式标签

```html
<font属性=“属性值”>文本内容</font>
```

### 表格

```html
<table border="1px">  //边框1像素
	<tr>
		<td>单元格内的文字</td>
	</tr>
    <tr></tr>
</table>
//几对tr 几行
```

### 表单

```html
用户输入信息的区域{ 
表单域 ：容纳控件和信息
表单控件：文本、多选。。。输入选择信息
提示信息：
}
```

#### 表单域

```html
<form action="url地址" method = "提交方式" name = "表单名称">
各种表单控件
</form>

method:get和post两个值 默认get，post安全+数据量大
```

#### 控件

```html
radio 单选框
<input type= "radio"name ="gender"value = "male"/>
<input type= "radio"name ="gender"value = "female"/> 
//name要相同才是单选
```

```
checkbox 复选框
```

```html
<td align ="right"> ... </td> 右对齐

<td colspan="2" align ="center">
	<input ..>
	<input ..>
</td>合并两列，居中
```

```html
<textarea cols="60" rows="5"> 评论框
```

### 无序列表

```html
<ul>
	<li type="disc">列表项1</li>
	<li type="square">列表项2</li>
	<li type="circle">列表项3</li>
</ul>//不推荐
```

### 有序标签

```html
<ol>
	<li >列表项1</li>
	<li >列表项2</li>
	<li >列表项3</li>
</ol> //不推荐
```

### 列表标签

```html
<dl>
	<dt>标签</dt>
		<dd>介绍</dd>
	<dt>标签</dt>
		<dd>介绍</dd>
</dl>
```

### 超链接

```html
<a href="跳转目标"target="目标窗口弹出方式">文本或图案</a>
_blank 新窗口打开 推荐
```

### 图像标签

```html
<img src="images/0.jpg">
//不在images前面写"/" 表示在当前工程文件查找
。/当前文件所在目录
。。/上级目录
```

### Div标签

标记简单而言就是一个区块容器标记，可以将网页分割为独立的、不同的部分，以实现网页的规划和布局。

在<div>与</div>之间可以容纳段落、标题、图像等各种网页元素，也就是说大多数HTML标记都可以嵌套在<div>标记中，并且<div>还可以嵌套多层<div>。

## CSS

选择器{属性1:属性值1; 属性2:属性值2; 属性3:属性值3;…}

### 颜色

> 1、sanyuanse
>
> 2、十六进制：  #FF2343
>
> 3、RGB代码： rgb（255，0，0）

```html
如：超链接
a{
	font-size:18px;
}
```

### 类选择器

```html
<style>
  .one{
	font-family:宋体;
	font-size:24px;
 	color:red;
}
  .two{
	font-family:黑体;
	font-size:16px;
 	color:green;
}
</style>


<body>
	<h1 class="one">应用了类别选择器1</h1>
	<p class="one">应用了类别选择器1</p>
	<h2 class="two">应用了类别选择器2</h2>
</body>

```

### ID选择器

id选择器使用**“#”**进行标识，后面**紧跟id名**，页面中唯一的（一般不能复用）

```html
<style>
#first {
    font-size: 18px;
}
#second {
   font-size: 24px;
   color:red;
}
</style>

<body>
	<p id="first">id选择器1</p>
	<p id="second">id选择器2</p>	
</body>

```

### 通配符选择器

**“*”**号表示，它是所有选择器中作用范围最广的，能匹配页面中所有的元素。

*{属性1:属性值1; 属性2:属性值2; 属性3:属性值3; }

除了类、ID，其他全部网页属性都使用该属性，（不推荐）

### 行内式

```html
<h1 style="font-size:20px; color :blue; ">
   使用CSS行内式修饰一级标题的字体大小和颜色
</h1>
```

### 内嵌式

将CSS代码集中写在HTML文档的<head>头部标签中，并用<style>标签定义

<style>标签一般位于<head>标签中的<title>标签之后
    提前被加载和解析

```html
<head>
   <style>
	选择器 {属性1:属性值1; 属性2:属性值2; 属性3:属性值3;}
   </style>
</head>
```

### 外链式（链入式）

将所有的样式放在一个或多个以**.css**为扩展名的外部样式表文件中，通过<link />标签将外部样式表文件链接到HTML文件中。

```html
<head>
      <link href="CSS文件的路径" type="text/css" rel="stylesheet" />
</head>
```

- href：定义所链接外部样式表文件的地址，可以是相对路径，也可以是绝对路径。
- type：定义所链接文档的类型，这里需要指定为“text/css” 。
- rel：定义当前文档与被链接文档之间的关系，这里需要指定为“stylesheet”，表示被链接的文档是一个样式表文件。

## CSS+DIV

内容、

内边距（padding）、

边框（border）

外边距（margin）组成。

![image-20240312060225598](C:\Users\WangTianyang\AppData\Roaming\Typora\typora-user-images\image-20240312060225598.png)

### 边距属性

```html
margin:0 auto  上下外边距0,左右居中
```

### 设置背景颜色background-color

### 设置背景图像

```html
body
{
background-color:#CCC; 
background-image:url(images/bg.jpg);
}   

```

### 背景图像平铺

background-repea

| **平铺属性值** | **含义**                                               |
| -------------- | ------------------------------------------------------ |
| **repeat**     | **沿水平和竖直两个方向平铺（默认值）**                 |
| **no-repeat**  | **不平铺（****图像位于元素的左上角****，只显示一次）** |
| **repeat-x**   | **只沿水平方向平铺**                                   |
| **repeat-y**   | **只沿竖直方向平铺**                                   |

### 背景图像位置

background-position

### 背景图像固定

background-attachment

| **固定属性取值** | **含义**                                 |
| ---------------- | ---------------------------------------- |
| **scroll**       | **图像随页面元素一起滚动（默认值）。**   |
| **fixed**        | **图像固定在屏幕上，不随页面元素滚动。** |

### \<b>\<i>\<u>

**asd**    *faga*       加粗,斜体,下划线