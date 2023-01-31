# CSS学习笔记
<!-- TOC -->

- [CSS学习笔记](#css学习笔记)
  - [CS语法规则](#cs语法规则)
  - [CSS选择器](#css选择器)
    - [基本选择器](#基本选择器)
      - [通用选择器](#通用选择器)
      - [标签选择器](#标签选择器)
      - [ID选择器](#id选择器)
      - [类选择器](#类选择器)
    - [高级选择器](#高级选择器)
      - [后代选择器](#后代选择器)
      - [子代选择器](#子代选择器)
      - [相邻选择器](#相邻选择器)
      - [通用相邻选择器](#通用相邻选择器)
      - [分组选择器](#分组选择器)
      - [属性选择器](#属性选择器)
    - [伪类选择器](#伪类选择器)
  - [HTML引用CSS方法](#html引用css方法)
    - [内嵌样式](#内嵌样式)
    - [内联样式](#内联样式)
    - [外部样式](#外部样式)
    - [导入样式](#导入样式)
  - [CSS长度单位](#css长度单位)
    - [相对长度单位](#相对长度单位)
    - [绝对长度单位](#绝对长度单位)
  - [CSS属性：文本、字体、颜色、背景、链接、鼠标](#css属性文本字体颜色背景链接鼠标)
    - [文本样式](#文本样式)
    - [字体样式(font)](#字体样式font)
      - [font-family：设置字体](#font-family设置字体)
      - [font-style：设置字体的风格，例如倾斜、斜体](#font-style设置字体的风格例如倾斜斜体)
      - [font-weight：设置字体粗细](#font-weight设置字体粗细)
      - [font-size：设置字体尺寸](#font-size设置字体尺寸)
      - [font-variant：将小写字母转换为小型大写字母](#font-variant将小写字母转换为小型大写字母)
      - [font：字体属性的缩写，可以在一个声明中设置多个字体属性](#font字体属性的缩写可以在一个声明中设置多个字体属性)
      - [颜色样式](#颜色样式)
    - [背景样式](#背景样式)
      - [background-color：设置元素的背景颜色](#background-color设置元素的背景颜色)
      - [background-image：设置元素的背景图像](#background-image设置元素的背景图像)
      - [background-repeat：控制背景图像是否重复](#background-repeat控制背景图像是否重复)
      - [background-attachment：控制背景图像是否跟随窗口滚动](#background-attachment控制背景图像是否跟随窗口滚动)
      - [background-position：控制背景图像在元素中的位置](#background-position控制背景图像在元素中的位置)
      - [background-origin：设置 background-position 属性相对于什么位置来定位背景图像](#background-origin设置-background-position-属性相对于什么位置来定位背景图像)
      - [background-size：设置背景图像的尺寸](#background-size设置背景图像的尺寸)
      - [background-clip：设置背景图像的显示区域](#background-clip设置背景图像的显示区域)
      - [background：背景属性的缩写，可以在一个声明中设置所有的背景属性](#background背景属性的缩写可以在一个声明中设置所有的背景属性)
    - [链接样式](#链接样式)
    - [鼠标样式](#鼠标样式)
    - [精灵图](#精灵图)
  - [CSS属性：盒子模型](#css属性盒子模型)
    - [内容区（content）](#内容区content)
    - [边框](#边框)
      - [border-style：设置边框的样式，例如实线、虚线等](#border-style设置边框的样式例如实线虚线等)
      - [border-width：设置边框的宽度（厚度）](#border-width设置边框的宽度厚度)
      - [border-color：设置边框的颜色](#border-color设置边框的颜色)
      - [border：上面三个边框属性的缩写](#border上面三个边框属性的缩写)
    - [边框图片 border-image](#边框图片-border-image)
      - [border-image-source 定义边框图像的路径](#border-image-source-定义边框图像的路径)
      - [border-image-slice 分割图像](#border-image-slice-分割图像)
      - [border-image-width 设置图像宽度](#border-image-width-设置图像宽度)
      - [border-image-outset](#border-image-outset)
      - [border-image-repeat](#border-image-repeat)
    - [外边距(margin)](#外边距margin)
      - [外边距设置](#外边距设置)
      - [外边距折叠](#外边距折叠)
    - [内边距（padding）](#内边距padding)
    - [宽度和高度](#宽度和高度)
      - [width 设置元素内容区的宽度](#width-设置元素内容区的宽度)
      - [height 定义元素内容区的高度](#height-定义元素内容区的高度)
      - [max-width 和 max-height 设置元素内容区的最大宽度和最大高度](#max-width-和-max-height-设置元素内容区的最大宽度和最大高度)
      - [min-width 和 min-height 设置元素内容区的最小宽度和最小高度](#min-width-和-min-height-设置元素内容区的最小宽度和最小高度)
    - [轮廓](#轮廓)
      - [outline-color 设置轮廓的颜色](#outline-color-设置轮廓的颜色)
      - [outline-style 设置轮廓得样式](#outline-style-设置轮廓得样式)
      - [outline-width 设置轮廓的宽度](#outline-width-设置轮廓的宽度)
      - [outline](#outline)
      - [outline-offset](#outline-offset)
    - [盒子阴影（box-shadow）](#盒子阴影box-shadow)
    - [圆角（border-radius）](#圆角border-radius)
    - [box-sizing：设置盒子模型大小](#box-sizing设置盒子模型大小)
  - [CSS属性：布局](#css属性布局)
    - [可见性(visibility)](#可见性visibility)
    - [显示类型(display)](#显示类型display)
    - [浮动(float)](#浮动float)
    - [定位(position)](#定位position)
      - [static](#static)
      - [relative](#relative)
      - [absolute 绝对定位](#absolute-绝对定位)
      - [fixed 固定定位](#fixed-固定定位)

<!-- /TOC -->
## CS语法规则

```css
选择器{
    属性：值;
}
```

有三部分构成：

- 选择器
- 属性
- 值

## CSS选择器

选择器由 HTML 标签的 id、class 属性或标签本身以及一些特殊符号构成，用来指定要为哪个 HTML 元素定义样式。

### 基本选择器

#### 通用选择器

选择器用星号`*`表示，匹配 HTML 文档中的每个元素。在开发中，我们通常使用通用选择器来清除 HTML 元素中默认的内外边距。

```css
*{
    margin: 0 auto;
    padding:0;
}
```

#### 标签选择器

通过具体的标签名称来匹配文档内<font color='red'>所有同类</font>的标签

```css
标签名{
    属性：值;
}
```

#### ID选择器

用来匹配 HTML 文档中具有<font color='red'>指定 ID 属性的标签</font>，ID 选择器的定义需要用到井号`#`，后面紧跟 ID 属性的值

```css
#id值{
    属性：值;
}
```

#### 类选择器

用来匹配 HTML 文档中具有<font color='red'>指定 class 属性的所有标签</font>，选择器的定义需要用到一个英文的句号`.`，后面紧跟 class 属性的值。

```css
.class值{
    属性：值
}
```

又由于html里 class 属性可以不是唯一的，并且可以应用于不同类型的标签，因此还可以在定义类选择器时指定具体类型的标签`标签名.class属性值`

### 高级选择器

#### 后代选择器

一个标签2嵌套在一个标签1内部的时候，就可以将这个标签看1作是标签2的后代。

后代选择器的定义方式就是将`标签名、class 属性或 id 属性`等按照标签的嵌套关系由外到内的依次罗列，中间使用空格分开

```css
ul li a {
    text-decoration: none;
}
```

#### 子代选择器

子选择器与后代选择器类似，<font color='red'>不过子选择器只会匹配某个元素的直接后代</font>（元素与其子元素之间只有一层嵌套关系）。

子选择器由两个或多个选择器组成，选择器之间用大于号>分隔开：

```css
p>strong{
    color:red;
}
```

#### 相邻选择器

用来匹配某个元素<font color='red'>之后紧邻</font>的另一个元素，这两个元素拥有同一个父级元素并且不存在嵌套关系。

邻兄弟选择器的定义需要用到加号+，加号两边为相邻的两个元素。

```css
/*
h1 + p选择器会匹配同一父级下紧邻<h1>标签并在其后的<p>标签
*/
h1 + p {
    color: blue;
    font-size: 18px;
}
/*
ul.task + p选择器则会匹配同一父级下紧邻<ul>标签并在其后的<p>标签，
但<ul>要具有class="task"属性。
*/
ul.task + p {
    color: #f0f;
    text-indent: 30px;
}
```

#### 通用相邻选择器

用来匹配某个元素<font color='red'>之后</font>的另一个元素，<font color='red'>无需紧邻</font>，这两个元素拥有同一个父级元素并且不存在嵌套关系。

定义需要用到波浪号`~`，波浪号两边为同一父级元素下的两个元素，选择器会匹配波浪号后面的元素，如下所示：

```css
/*
h1 ∼ p选择器会匹配同一父级元素下<h1>标签之后的所用<p>标签。
*/
h1 ∼ p {
    color: blue;
    font-size: 18px;
}
```

#### 分组选择器

分组选择器可以将<font color='red'>同样的样式规则应用到多个选择器</font>中，每个选择器之间使用逗号`,`进行分隔，这么做可以避免定义重复的样式规则，最大程度地减少 CSS 样式表中的代码。

```css
/*
选择器h1、h2、h3中包含相同的样式font-weight: normal;
*/
h1, h2, h3 {
    font-weight: normal;
}
```

#### 属性选择器

用来匹配具有特定属性的元素。

属性选择器的定义方式与标签选择器相似，只不过需要在标签的后面使用方括号`[ ]`来指定标签具有的属性信息

``` css
/*
input[type="text"]选择器会匹配所有具有type="text"属性的<input>标签。

*/
input[type="text"] {
   color: blue;
}
```

方括号[ ]内的属性信息还支持以下几种写法：

- [target]：选择所有带有target属性元素；
- [target=_blank]：选择所有具有target="_blank" 属性的元素；
- [title~=flower]：选择title属性包含单词“flower”的所有元素；
- [lang|=en]：选择lang属性正好是“en”或以“en”为开头的所有元素。

### 伪类选择器

伪类是 W3C 制定的一套选择器的特殊状态，通过伪类可以设置元素的动态状态，例如悬停（hover）、点击（active）以及文档中不能通过其它选择器选择的元素（这些元素没有 ID 或 class 属性），例如第一个子元素（first-child）或者最后一个子元素（last-child）。

伪类的名称不区分大小写，但需要以冒号`:`开头。另外，伪类需要与 CSS 中的选择器结合使用，语法格式如下：

```css
selector:pseudo-class {
    property: value;
}
```

![伪类](%E4%BC%AA%E7%B1%BB.png)

## HTML引用CSS方法

### 内嵌样式

在HTML文件`<head>`标签内的`<style>`标签中定义CSS样式。

```html
<!DOCTYPE html>
<html>
    <head>
        <title>编程帮</title>
        <style>
            /*
            定义CSS样式
            */
            body {
                background-color: linen;
            }
            h1 {
                color: maroon;
                margin-left: 40px;
            }
        </style>
    </head>  
    <body>
        <h1>编程帮</h1>
        <p>http://www.biancheng.net/</p>
    </body>
</html>
```

### 内联样式

将CSS样式定义在HTML的标签`style`属性中。

由于内联样式定义在标签内部，所以它只对所在的标签有效。

内联样式虽然可以很方便的为 HTML 标签赋予 CSS 样式，但它的缺点也非常明显，不推荐过多使用。

>- 定义内联样式需要在每个 HTML 标签中定义 style 属性，很不方便；
>- 在内联样式中定义的样式不能再其它任何地方重用；
>- 内联样式在后期维护时很不方便，因为一个网站通常有很多页面组成，当修改页面样式时需要对页面逐个修改；
>- 添加过多的内联样式会导致 HTML 文档的体积增大。

```html
<!DOCTYPE html>
<html>
    <head>
        <title>编程帮</title>
    </head>  
    <body>
        /*
        定义了h1和p两个标签的样式
        */
        <h1 style="color: maroon; margin-left: 40px">编程帮</h1>
        <p style="color: blue;">http://www.biancheng.net/</p>
    </body>
</html>
```

### 外部样式

外部样式表是<font color='red'>最推荐的</font>引用 CSS 的方式.

只需要将 CSS 样式定义在一个 .css 格式的文件中，然后在HTML 的头部使用`<link>`标签将这个 .css 格式的样式文件应用到 HTML 文档中。

`<link>href="css文件地址" type="连接文档的类型" rel="定义链接外部文件的关联类型" </link>`

```html
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <link href="lianjie.css" type="text/css" rel="stylesheet" />
    <link href="lianjie-2.css" type="text/css" rel="stylesheet" />
  </head>
  <body>
  </body>
</html>
```

### 导入样式

在HTML文件的头部`<style>`标签内使用@import来引用外部样式表，语法格式为

```html
<style>
    @import "CSS文件地址"
</style>
```

## CSS长度单位

设置某些属性值时可能会涉及到与值对应的单位，根据类型的不同可以分为两类，分别是绝对长度单位（例如英寸、厘米、点）和相对长度单位（例如百分比）。

### 相对长度单位

相对长度单位指的是这个单位没有一个固定的值，它的值受到其它元素属性（例如浏览器窗口的大小、父级元素的大小）的影响，在响应式布局方面相对长度单位非常适用。

|单位|描述|实例|
---|---|---
em|相对于自身 font-size（字体大小）属性的值，如果自身没有设置，则继承父元素 font-size 属性的值，1em 等同于 font-size 属性值|p{line-height:2em;}
rem|相对于根元素<html>的 font-size 属性的大小|p{font-size: 1.2rem;}
ex|相对于所用字体中小写英文字母 x 的高度，若无法确定 x 的高度则使用 0.5em 计算|p{font-size: 1ex;}
ch|相对于所用字体中数字 0 的高度，若无法确定 0 的高度则使用 0.5em 计算|p{line-height: 3ch}
vw|相对于浏览器宽度，1vw=1%|p{font-size: 5vw;}
vh|相对于浏览器的高度，1vh = 窗口高度的 1%|p{font-size: 5vh;}
vmin|w 与 vh 中较小的值|p{font-size: 5vmin;}
vmax|vw 与 vh 中较大的值|p{font-size: 5vmax;}
%|相对于父元素的宽度或高度百分比|div{width: 55%}

### 绝对长度单位

绝对长度单位表示一个真实的物理尺寸，它的大小是固定的，不会因为其它元素尺寸的变化而变化。

单位|描述
---|---
cm|厘米
mm|毫米
in|英寸（1in = 96px = 2.54cm）
px|像素(1px = 1/96in）
pt|磅(1pt = 1/72in）
pc|派卡（1pc = 12pt)

## CSS属性：文本、字体、颜色、背景、链接、鼠标

### 文本样式

>- text-align：设置文本的水平对齐方式；
>- text-decoration：设置文本的装饰；
>- text-transform：设置文本中英文的大小写转换方式；
>- text-indent：设置文本的缩进方式；
>- line-height：设置行高；
>- letter-spacing：设置字符间距；
>- word-spacing：设置单词与单词之间的间距（对中文无效）；
>- text-shadow：设置文本阴影；
>- vertical-align：设置文本的垂直对齐方式；
>- white-space：设置文本中空白的处理方式；
>- direction：设置文本方向。

通过 CSS 中的文本属性可以像操作 Word 文档那样定义网页中文本的字符间距、对齐方式、缩进等

属性|描述|值
---|---|---
text-align|水平对齐方式|<p>1. left 默认值 左对齐</p><p>2.right 右对齐</p><p>3.center 居中对齐</p><p>4.justify 居中对齐</p><p>5.inherit 从父元素继承`text-align`属性值</p>
vertical-align|垂直对齐方式|<p>1.baseline 默认值，将元素的基线与父元素的基线对齐</p><p>2.sub 下标对齐，将元素的基线相对于父元素的基线降低</p><p>3.super 上标对齐，将元素的基线相对于父元素的基线升高</p><p>4.top 顶部对齐，将元素行内框的顶端与行框的顶端对齐</p><p>5.text-top 文本顶部对齐，把元素的顶端与父元素字体的顶端对齐</p><p>6.middle 居中对齐，通常使用在图片上，将图片垂直方向的中线与文本的中线（文字元素行内框的中线）对齐</p><p>7.bottom 底部对齐，将元素行内框的顶端与行框的底端对齐</p><p>8.length 以数字加单位的形式设置元素基线距离父元素基线的距离（可以为负值）</p><p>9.length 以数字加单位的形式设置元素基线距离父元素基线的距离（可以为负值</p><p>10.% 使用 "line-height" 属性的百分比值来排列此元素，允许使用负值</p><p>11.nherit 从父元素继承 vertical-align 属性的值</p>
text-decoration|设置或删除文本装饰|<p>1.none 默认值，标准文本，没有额外装饰，可以用来删除已有的文本装饰</p><p>2.underline 在文本下方添加一条下滑线</p><p>3.overline在文本上方添加一条上滑线</p><p>4.line-through在文本中间定义一条线，类似于删除线</p><p>5.inherit从父元素继承 text-decoration 属</p>
text-transform|来控制文本中英文字母的大小写|<p>1.none 默认值，对原文不做更改</p><p>2. capitalize将文本中的每个单词更改为以大写字母开头的形式</p><p>3.uppercase将文本中的英文字母全部更改为大写</p><p>4.lowercase将文本中英文字母全部变更为小写</p><p>5.inherit 继承父类元素属性值</p>
text-indent|首行缩进|<p>1.固定长度&emsp;以固定的值加单位的形式（例如 2em）定义缩进距离，默认值为 0</p><p>2.相对长度 &emsp;以基于父元素宽度的百分比来定义缩进距离</p><p>3. inherit 继承父类元素属性值</p>
line-height|行高|<p>1.normal默认值</p><p>2.number以具体的数字设置行高，这个数字会与当前的字体大小相乘，并将得到的值设置为行高</p><p>3.length以数字加单位的形式设置固定的行高</p><p>4.%以百分比的形式设置基于当前字体尺寸百分比的行高</p><p>5.inherit从父元素继承 line-height 属性的值</p>
letter-spacing|设置字符间的间距|<p>1.normal 默认值</p><p>2.length固定长度设置间距</p><p>3.inherit从父标签继承</p>
word-spacing|设置单次之间的间距，对中文无效|<p>1.normal 默认值</p><p>2.length固定长度设置间距</p><p>3.inherit从父标签继承</p>
text-shadow|为文本添加阴影及模糊效果|语句格式：<p><code>text-shadow: h-shadow v-shadow blur color;</code></p><p>h-shadow：必填值，设置阴影的水平位置，允许为负值</p><p>v-shadow：必填值，设置阴影的垂直位置，允许为负值；</p><p>blur：可选值，设置模糊的距离；</p><p>color：可选值，设置阴影的颜色</p>
white-space|设置如何处理元素内的空白|<p>1.normal 默认值，忽略文本中的空白</p><p>2.pre  保留文本中的空白，类似于`<pre>`标签的效果</p><p>3.nowrap 文本会在一行中显示，不会自动换行，直到遇到`<br>`标签为止</p><p>4.pre-wrap 保留文本中的空白，但是正常地进行换行</p><p>5.pre-line 合并文本中的空白，但是保留换行符</p><p>6.inherit 从父元素继承 white-space 属性的值</p>
direction|设置文本的方向|<p>1.ltr 默认值，文本按从左到右的方向输出</p><p>2.rtl 文本按从右到左的方向输出</p><p>3.inherit 从父元素继承 direction 属性的值</p>

### 字体样式(font)

#### font-family：设置字体

值|描述
---|---
family-name、generic-family|family-name：字体名称；generic-family：字体族，也就是某种类型的字体组合。字体的默认值取决于浏览器设置
inherit|从父元素继承字体的设置
>在网页设计中最常用的字体族是 serif 和 sans-serif，因为它们适合阅读。在显示一些程序代码是通常使用等宽字体，这样可以使用程序代码看起来更加工整。

#### font-style：设置字体的风格，例如倾斜、斜体

值|描述
---|---
normal|默认值，文本以正常字体显示
italic|斜体
oblique|文本倾斜，可以处理没有斜体的字体
inherit|继承父类元素

#### font-weight：设置字体粗细

值|描述
---|---
normal|默认正常
bold|粗体
bolder|更粗体
lighter|更细体
100、200、...、900|由细到粗的设置字体粗细，100 为最细的字体，400 等同于 normal，700 等同于 bold
inherit|继承父类

#### font-size：设置字体尺寸

值|描述
---|---
xx-small、x-small、small、medium、large、x-large、xx-large|以关键字的形式把字体设置为不同的大小，从 xx-small 到 xx-large 依次变大，默认值为 medium
smaller|为字体设置一个比父元素更小的尺寸
larger|为字体设置一个比父元素更大的尺寸
length| 以数值加单位的形式把字体设置为一个固定尺寸，例如 18px、2em
%|以百分比的形式为字体设置一个相对于父元素字体的大小
inherit|继承父类

#### font-variant：将小写字母转换为小型大写字母

值|描述
---|---
normal| 默认值，浏览器会显示一个标准的字体
small-caps| 将文本中的小写英文字母转换为小型大写字母
inherit| 从父元素继承 font-variant 属性的值

#### font：字体属性的缩写，可以在一个声明中设置多个字体属性

使用 font 属性需要遵循以下顺序：

```css
选择器{
    font：font-style font-variant font-weight font-size/line-height font-family
    }
```

>在使用 font 属性时，有以下几点需要注意：
>
>- 使用 font 属性时必须按照如上所示的顺序，并且 font-size 和 font-family 两个属性不可忽略；
>- font 属性中的每个参数仅允许设置一个值，除 font-size 和 font-family 属性外，被忽略的属性将被设置为各自的默认值；
>- 若要定义 line-height 属性，则需要使用斜线/将 font-size 和 line-height 属性分开。

#### 颜色样式

CSS 中提供了一些属性（例如 color、background）来设置 HTML 元素的颜色（例如元素的背景颜色或字体颜色），可以通过不同形式的值来指定颜色，如下表所示：

值 |描述| 实例
---|---|---
颜色名称| 使用颜色名称来设置具体的颜色，比如 red、blue、brown、lightseagreen 等，颜色名称不区分大小写 |color: red;
十六进制码| 使用十六进制码以 #RRGGBB 或 #RGB（比如 #ff0000）的形式设置具体颜色，"#" 后跟 6 位或 3 位十六进制字符（0-9, A-F）| color: #f03;
RGB |通过 rgb() 函数对 red、green、blue 三原色的强度进行控制，从而实现不同的颜色 |color: rgb(255,0,51);
RGBA |RGBA 扩展了 RGB，在 RGB 的基础上增加了 alpha 通道来设置颜色的透明度，需要使用 rgba() 函数实现| color: rgba(255,0,0,0.1);
HSL| 通过 hsl() 函数对颜色的色调、饱和度、亮度进行调节，从而实现不同的颜色 |color: hsl(120,100%,25%);
HSLA| HSLA 扩展了 HSL，在 HSL 的基础上增加了 alpha 通道来设置颜色的透明度，需要使用 hsla() 函数实现 |color: hsla(240,100%,50%,0.5);

### 背景样式

CSS 中提供了一系列用于设置 HTML 元素背景效果的属性，如下所示：

#### background-color：设置元素的背景颜色

#### background-image：设置元素的背景图像

默认情况下浏览器会从元素内容的左上角开始（若有内边距则从元素内边距区域的左上角开始），在水平和垂直方向上重复背景图像，以填充整个元素区域，可以使用 background-repeat 属性来控制背景图像是否重复或如何重复。

值 |描述
---|---
url('URL')|指向图像的路径
none |默认值，不显示背景图像
inherit |从父元素继承背景图像的设置

#### background-repeat：控制背景图像是否重复

值 |描述
---|---
repeat |默认值，背景图像将在垂直方向和水平方向上重复
repeat-x| 背景图像仅在水平方向上重复
repeat-y| 背景图像仅在垂直方向上重复
no-repeat| 背景图像仅显示一次，不在任何方向上重复
inherit |从父元素继承 background-repeat 属性的设置

#### background-attachment：控制背景图像是否跟随窗口滚动

值 |描述
---|---
scroll| 默认值，背景图像随着页面元素的滚动而移动
fixed |当页面的其余部分滚动时，背景图像固定不动
inherit |从父元素继承 background-attachment 属性的设置

#### background-position：控制背景图像在元素中的位置

值 |描述
---|---
left top（左上）、left center（左中）、left bottom（左下）、right top（右上）、right center（右中）、right bottom（右下）、center top（中上）、center center（居中）、center bottom（中下）| 使用一些关键词表示背景图像的位置，如果您仅设置第一个关键词，那么第二个将默认为 center
x% y%| 使用百分比表示背景图像距离元素左上角的距离，x% 为水平方向，y% 为垂直方向，左上角为 0% 0%，右下角是 100% 100%，如果您仅设置第一个值，那么另一个值将是 50%，默认值为 0% 0%
xpos ypos| 使用像素（px）或者其它 CSS 单位表示背景图像距离元素左上角的距离，xpos 为水平方向，ypos 为垂直方向，左上角为 0px 0px，右下角视元素的尺寸而定，百分比和单位的形式可以混用，如果您仅设置第一个值，那么另一个值将默认为 50%

#### background-origin：设置 background-position 属性相对于什么位置来定位背景图像

在使用 background-position 属性来设置背景图像的位置时，默认是以<font color='red'>元素左上角的位置</font>来计算的。可以使用 background-origin 属性来设置 background-position 属性相对哪个位置来定位背景图像
值|描述
---|---
padding-box|相对于元素的内边距区域来定位背景图像
border-box|相对于元素的边框区域来定位背景图像
content-box|相对于元素的内容区域来定位背景图像

#### background-size：设置背景图像的尺寸

值|描述
---|---
xpos ypos| 使用像素（px）或其它 CSS 单位来设置背景图像的高度和宽度，xpos 表示宽度，ypos 表示高度，如果只设置第一个值，那么第二个值将被设置为默认值 auto（自动）
x% y% |使用百分比表示背景图像相对于所在元素宽度与高度的百分比，x% 表示宽度，y% 表示高度，如果只设置第一个值，那么第二个值将被设置为默认值 auto（自动）
cover| 保持背景图像的横纵比例并将图像缩放至足够大，使背景图像可以完全覆盖元素所在的区域，这么做可能会导致背景图像的某些部分超出元素区域而无法显示
contain| 保持背景图像的横纵比例并将图像缩放至足够大，使背景图像可以完整的显示在元素所在区域，背景图像可能无法完全覆盖整个元素区域

#### background-clip：设置背景图像的显示区域

值|描述
---|---
border-box| 默认值，在元素边框及以内的区域显示背景图像
padding-box| 在元素内边距及以内的区域显示背景图像
content-box |在元素内容区域显示背景图像

#### background：背景属性的缩写，可以在一个声明中设置所有的背景属性

```css
background: background-color  background-image  background-position/ background-size background-repeat  background-attachment  background-origin background-clip
```

>- 每个属性之间使用空格进行分隔；
>- 如果同时设置 background-position 和 background-size 属性，这两个属性之间需要使用斜线/分隔，并且需要遵循 background-position 属性在前 background-size 属性在后的顺序；
>- 如果同时设置 background-origin 和 background-clip 属性，需要遵循 background-origin 属性在前 background-clip 属性在后的顺序。如果 background-origin 与 background-clip 属性的值相同，则可以只设置一个值。

### 链接样式

链接有四种不同的状态，分别是 link、visited、active 和 hover，可以通过以下<font color='red'>伪类选择器</font>来为链接的四种状态设置不同的样式：

- link：定义普通或未访问链接的样式；
- visited：定义已经访问过链接的样式；
- hover：定义当鼠标经过或悬停在链接上时的样式；
- active：定义点击链接时的样式。

通过上面的四个伪类选择器，您可以像给普通文本定义样式那样，为链接定义任何想要的 CSS 样式，例如颜色、字体、背景、边框等。
>注意：在定义四个伪类选择器时需要按照一定的顺序，一般情况下:hover必须位于:link和:visited之后，:active必须位于:hover之后。

### 鼠标样式

在浏览网页的过程中，当我们将鼠标移动到一些元素上时，鼠标的样式会发生相应的改变，例如当鼠标指向文本时，鼠标的样式会变成类似大写字母I的样子；当鼠标指向链接时，鼠标会变成一个小手的形状等。

除了这些默认的变化外，可以通过 CSS 中的 `cursor` 属性来改变网页中鼠标（光标）的样式。

<a href='http://c.biancheng.net/css3/cursor.html'>cursor值参考链接</a>

### 精灵图

参考链接：<a href="https://blog.csdn.net/wangwenkai76/article/details/82556642">CSS精灵图（sprite）</a>

## CSS属性：盒子模型

盒子模型是网页设计中经常用到的一种思维模型，由四个部分构成，从内到外分别为内容区（content）、内边距（padding）、边框（border）和外边距（margin），CSS 为这四个部分提供了一系列相关属性，通过对这些属性的设置可以丰富盒子的表现效果。

网页中的每个元素都可以看作是如下图所示一个盒子模型：

![盒子模型](%E7%9B%92%E5%AD%90%E6%A8%A1%E5%9E%8B.gif "盒子模型")

### 内容区（content）

内容区是整个盒子模型的中心，其中存放了盒子的主要内容，这些内容可以是文本、图像等资源。

内容区有 width、height、overflow 三个属性，其中 width 和 height 属性用来指定盒子内容区域的宽度和高度，当内容信息过多，超出内容区所设置的范围时，则可以使用<font color='red'>滚动样式条 overflow </font>属性设置溢出内容的处理方式。

overflow 属性有四个可选值：

- hidden：表示隐藏溢出的部分；
- visible：表示显示溢出的部分（溢出的部分将显示在盒子外部）；
- scroll：表示为内容区添加一个滚动条，您可以通过滑动这个滚动条来查看内容区的全部内容；
- auto：表示由浏览器决定如何处理溢出部分。

### 边框

CSS 中的边框是围绕着元素内容和内边距的一条或多条线段，可以自定义这些线段的样式、宽度以及颜色。

#### border-style：设置边框的样式，例如实线、虚线等

border-style 属性用来设置元素中<font color='red'>所有边框</font>的样式，或者属性用来设置元素中<font color='red'>单独为某个边框</font>设置样式，其语法格式如下：

```css
/*顺序为：上右下左*/
border-style: border-top-style  border-right-style  border-bottom-style  border-left-style;
```

border-style 属性的可选值如下
值|描述
---|---
none|无边框
hidden|隐藏边框，与 "none" 类似
dotted|点状虚线边框
dashed|虚线边框
solid|实线边框
double|双边实线边框，双实线边框的宽度等于 border-width 的值
groove|定义 3D 凹槽边框，其效果取决于 border-color 的值
ridge|定义 3D 垄状边框,同上
inset|定义 3D 嵌入边框，同上
outset|定义 3D 突出边框，同上
inherit|父类继承

#### border-width：设置边框的宽度（厚度）

用来设置元素中所有边框的宽度，或者单独为某个边框设置宽度，其语法格式如下：

```css
/*顺序为：上右下左*/
border-width: border-top-width border-right-width border-bottom-width border-left-width;
```

可选值：
值|描述
---|---
thin| 定义较细的边框
medium| 默认值，定义中等宽度的边框
thick |定义较粗的边框
length |使用数值加单位的形式设置具体的边框宽度，例如 2px
inherit |从父元素继承边框的宽度

#### border-color：设置边框的颜色

用来设置元素中所有边框的颜色，或者单独为某个边框设置颜色，其语法格式如下：

```css
/*顺序为：上右下左*/
border-color: border-top-color border-right-color border-bottom-color border-left-color;
```

#### border：上面三个边框属性的缩写

法格式如下：

```css
border: border-width border-style border-color;
```

### 边框图片 border-image

 CSS3 中的 border-image 属性使用图像来作为元素的边框。

 border-image 属性将一副图像划分为 9 个单独的部分，浏览器会自动使用相应的部分来替换边框的默认样式。  
 border-image 属性是五个 border-image-* 属性的简写

```css
border-image：border-image-source  border-image-slice border-image-width border-image-outset  border-image-repeat
```  

#### border-image-source 定义边框图像的路径

none 为 border-image-source 属性的默认值，表示不使用图像来替换边框的默认样式；`<image>`为使用 url() 函数指定的图像路径`border-image-source:url("图像路径")`

#### border-image-slice 分割图像

语法格式如下：

```css
border-image-slice：[ <number> | <percentage> ]{1,4} && fill?
```

border-image-slice 属性可以接收三种类型的值：

- `number`：数值，用具体数值指定图像分割的位置，数值代表图像的像素位置或向量坐标，不允许负值；
- `percentage`：百分比，相对于图像尺寸的百分比，图像的宽度影响水平方向，高度影响垂直方向；
- `fill`：保留边框图像的中间部分。

> 除 fill 关键字外，border-image-slice 属性可以接受 1~4 个参数值：
>
>- 如果提供全部四个参数值，那么将按上、右、下、左的顺序对图像进行分割；
>- 如果提供三个参数，那么第一个参数用于上方，第二个参数用于左、右两侧，第三个参数用于下方；
>- 如果提供两个参数，那么第一个参数用于上方和下方，第二个参数用于左、右两个；
>- 如果只提供一个参数，那么上、右、下、左都将使用该值进行分割。

![分割图像](分割图像.gif)

#### border-image-width 设置图像宽度

设置通过 border-image-source 属性加载的图像厚度（宽度），属性的语法格式如下：

```css
border-image-width：[ <length> | <percentage> | <number> | auto ]{1,4}
```

语法说明如下：

- length：使用数值加单位的形式指定图像边框的宽度，不允许为负值；
- percentage：用百分比的形式指定图像边框的宽度，参照图像边框区域的宽和高进行换算，不允许负值；
- number：使用浮点数指定图像边框的宽度，该值对应border-width 的倍数，例如值为 2，则参数的实际值为 2 * border-width，不允许负值；border-image-width 属性的默认值为 1
- auto：由浏览器自动设定，当 border-image-width 设置为 auto 时，它的实际值与 border-image-slice 相同的值。

border-image-width 可以接受 1~4 个参数值：

- 四个参数值，按照上、右、下、左的顺序设置；
- 三个参数，第一个参数用于上边框，第二个参数用于左、右两个边框，第三个参数用于下边框；
- 两个参数，第一个参数用于上、下两个边框，第二个参数用于左、右两个边框；
- 一个参数，上、右、下、左都使用该值设置。

#### border-image-outset

定义图像边框相对于边框边界向外偏移的距离（使图像边框延伸到盒子模型以外）

```css
border-image-outset：[ <length> | <number> ]{1,4}
```

语法说明如下：

- length：用具体的数值加单位的形式指定图像边框向外偏移的距离，不允许为负值；
- number：用浮点数指定图像边框向外偏移的距离，该值表示 border-width 的倍数
  
border-image-outset 属性同样可以接受 1~4 个参数值：

- 提供四个参数值，那么将按上、右、下、左的顺序作用于四边；
- 提供三个参数值，那么第一个参数将用于上边框，第二个参数将用于左、右两个边框，第三个参数将用于下边框；
- 提供两个参数，那么第一个参数将用于上、下两个边框，第二个参数将用于左、右两个边框；
- 只提供一个参数，那么该参数将同时作用于四边。

#### border-image-repeat

设置如何填充使用 border-image-slice 属性分割的图像边框，例如平铺、拉伸等等，该属性的语法格式如下：

```css
border-image-repeat：[ stretch | repeat | round | space ]{1,2}
```

语法说明如下：

- stretch：将被分割的图像使用拉伸的方式来填充满边框区域；
- repeat：将被分割的图像使用重复平铺的方式来填充满边框区域，当图像碰到边界时，超出的部分会被截断；
- round：与 repeat 关键字类似，不同之处在于，当背景图像不能以整数次平铺时，会根据情况缩放图像；
- space：与 repeat 关键字类似，不同之处在于，当背景图像不能以整数次平铺时，会用空白间隙填充在图像周围。

border-image-repeat 属性能够接受 1~2 个参数值：

- 如果提供两个参数，那么第一个参数将用于水平方向，第二个将用于垂直方向；
- 如果只提供一个参数，那么将在水平和垂直方向都应用该值。

### 外边距(margin)

外边距（margin）是围绕在元素边框以外（不包括边框）的空白区域，这片区域不受 background 属性的影响，始终是透明的。

默认情况下如果不设置外边距属性，HTML 元素就是不会有外边距，但也有例外的情况，因为浏览器会为一些 HTML 元素设置默认的外边距，例如`<p>`元素。

![外边距演示](%E5%A4%96%E8%BE%B9%E8%B7%9D.png "外边距演示")

#### 外边距设置

可以使用下面的属性来为 HTML 元素设置外边距：

- margin-top：设置元素上方的外边距；
- margin-bottom：设置元素下方的外边距；
- margin-right：设置元素右侧的外边距；
- margin-left：设置元素左侧的外边距；
- margin：外边距的简写属性，可以同时设置元素四个方向（上下左右）的外边距。
  >这里需要特别说明一下 margin 属性，与其它几个属性不同，margin 属性可以接受 1~4 个参数（参数之间使用空格分隔）：
如果提供四个参数，那么将按照上、右、下、左的顺序分别作用于元素四个方向的外边距；
  >
  >- 如果提供三个参数，那么第一个参数会作用在元素上方的外边距，第二个参数会作用在元素左右两侧的外边距，第三个参数则作用在元素下方的外边距；
  >- 如果提供两个参数，那么第一个参数会作用在元素上方和下方的外边距，第二个参数会作用在元素的左右两侧的外边距；
  >- 如果只提供一个参数，那么这个值将同时作用于元素上下左右四个方向的外边距。

值| 描述
---|---
auto| 由浏览器计算外边距的尺寸
length| 使用具体数值配合 px、cm 等单位来定义元素外边距的尺寸，可以为负值，默认值为 0px
%| 定义基于父元素的宽度百分比的外边距，可以为负值
inherit| 从父元素继承外边距属性的值

#### 外边距折叠

外边距折叠指的是相邻的两个或多个外边距会在垂直方向上发生合并，合并为一个外边距。关于外边距折叠有以下几点需要注意：

- margin 折叠只发生在块级元素上；
- 浮动元素的外边距不会与任何外边距发生折叠；
- 设置了 overflow 属性且值不为 visible 的块级元素，将不会与它的子元素发生外边距折叠；
- 绝对定位元素的外边距不与任何外边距发生折叠；
- 根元素（例如`<body>`）的外边距不与其它任何外边距发生折叠。

### 内边距（padding）

是指元素内容区与边框之间的区域，与外边距不同，内边距会受到背景属性的影响。通过下面的属性来设置元素内边距的尺寸：

![内边距演示](内边距.png "内边距演示")

- padding-top：设置元素内容区上方的内边距；
- padding-right：设置元素内容区右侧的内边距；
- padding-bottom：设置元素内容区下方的内边距；
- padding-left：设置元素内容区左侧的内边距；
- padding：内边距属性的缩写形式，可以同时设置上下左右四个方向上的内边距。细节上与外边距一致。

值| 描述
---|---
length| 使用具体数值配合 px、cm 等单位来定义元素内边距的尺寸，不能为负值，默认值为 0px
% |定义基于父元素的宽度百分比的内边距，不能为负值
inherit| 从父元素继承内边距属性的值

### 宽度和高度

尺寸属性指的就是元素的宽度和高度属性，CSS 中提供了 width、height、max-width、min-width、max-height 和 min-height 等几个属性来设置元素的宽度和高度

#### width 设置元素内容区的宽度

可选值：
值| 描述
---|---
auto| 默认值，浏览器自动计算元素的实际宽度
length| 使用具体数值配合 px、cm 等单位来定义宽度
%| 定义基于父元素宽度百分比的宽度
inherit| 从父元素继承 width 属性的值

> 提示：对于`<img>`标签来说，若仅指定 width 属性，那么它的 height 属性将根据原图片尺寸进行等比例缩放。

#### height 定义元素内容区的高度

可选值：
值| 描述
---|---
auto| 默认值，浏览器自动计算元素的实际高度
length| 使用具体数值配合 px、cm 等单位来定义高度
%| 定义基于父元素宽度百分比的高度
inherit| 从父元素继承 height 属性的值

> 默认情况下，浏览器会将某些元素的宽度设置为 100%，例如`<div>、<p>`，而元素的高度则是根据元素中的内容来确定的，所以有些情况下您不必为元素设置固定的宽度或高度。

#### max-width 和 max-height 设置元素内容区的最大宽度和最大高度

定义了 max-width 和 max-height 属性时，不论 width 或 height 属性的实际值是多少，width 和 height 属性的实际值都会小于等于 max-width 和 max-height 属性的值。

可选值：
值| 描述
---|---
none| 默认值，不做限制
length| 使用具体数值配合 px、cm 等单位
%| 定义基于父元素宽度和高度百分比
inherit| 从父元素继承

> 以 max-width 属性为例：（max-height 属性的特性与之相似）
>
>- 当 max-width 属性的值小于 width 属性时，width 属性的值会被重新定义为与 max-width 属性相同的值；
>- 当 max-width 属性的值大于 width 时，max-width 属性将会被忽略；
>- 当 max-width 属性的值小于 min-width 时，max-width 属性将会被忽略。

#### min-width 和 min-height 设置元素内容区的最小宽度和最小高度

用法与最大类似

### 轮廓

轮廓（outline）是绘制于元素周围的一条线，位于边框的外围（紧贴着边框），主要用来突出显示某个元素，如下图所示：

![轮廓演示](%E8%BD%AE%E5%BB%93.gif "轮廓演示")

轮廓与边框的区别：

- 元素四个边框可以单独设置属性，而轮廓不能单独设置；
- 边框的宽度会直接影响元素的尺寸，而轮廓不会占用页面空间，不会影响页面的布局，但是轮廓会与页面上的其它元素发声重叠；
- 除了会与周围的元素发声重叠外，轮廓对周围的元素没有任何影响；
- 边框是元素尺寸的一部分，而轮廓不是，也就是说无论轮廓的宽度是多少，元素的尺寸都不会改变；
- 轮廓可以不是矩形的，但不能直接创建圆形轮廓。

#### outline-color 设置轮廓的颜色

#### outline-style 设置轮廓得样式

值| 描述
---|---
none| 默认值，没有轮廓
dotted| 定义点状的轮廓
dashed| 定义虚线轮廓
solid |定义实线轮廓
double |定义双实线轮廓，两条实线之间的宽度等同于 outline-width 的值
groove| 定义 3D 凹槽轮廓，具体效果取决于 outline-color 的值
ridge |定义 3D 凸槽轮廓，具体效果取决于 outline-color 的值
inset |定义 3D 凹边轮廓，具体效果取决于 outline-color 的值
outset |定义 3D 凸边轮廓，具体效果取决于 outline-color 的值
inherit| 从父元素继承轮廓样式的设置

#### outline-width 设置轮廓的宽度

只有当 outline-style 属性的值不为 none 时，outline-width 属性才会生效.

值| 描述
---|---
thin |设置较细的轮廓
medium |默认值，设置中等宽度的轮廓
thick |设置较粗的轮廓
length |使用具体数值加单位（px、em、cm 等）的形式设置轮廓的宽度
inherit |从父元素继承轮廓的宽度

#### outline

 outline 属性可以同时设置这三个属性中的一个或多个，语法格式如下：

 ```css
outline: outline-width outline-style outline-color;
```

#### outline-offset

默认情况下轮廓是紧贴着边框的，通过 outline-offset 属性可以设置轮廓与边框之间的距离，属性的可选值如下：

值 |描述
---|---
length |使用具体数值加单位的形式设置轮廓与边框之间的距离，可以为负值
inherit |从父元素继承 outline-offset 属性的值

### 盒子阴影（box-shadow）

可以为元素设置阴影效果

```css
box-shadow:  h-shadow v-shadow blur spread color inset;
```

语法说明如下：

- h-shadow：必填参数，设置阴影水平方向的偏移量，可以为负值；
- v-shadow：必填参数，设置阴影垂直方向的偏移量，可以为负值；
- blur：可选参数，设置模糊的半径，值越大，模糊越大，阴影的边缘越模糊，不允许使用负值；
- spread：可选参数，设置阴影的尺寸；
- color：可选参数，设置阴影的颜色；
- inset：可选参数，将默认的外部阴影 (outset) 改为内部阴影。

### 圆角（border-radius）

- border-top-left-radius：为元素左上角设置圆角效果；
- border-top-right-radius：为元素右上角设置圆角效果；
- border-bottom-right-radius：为元素右下角设置圆角效果；
- border-bottom-left-radius：为元素左下角设置圆角效果；
- border-radius：上面四个属性的简写形式，可以同时为元素的四个角设置圆角效果。

语法规则

```css
/*写法1
*值可取：
length 通过数值加单位的形式定义圆角的形状
percentage 以百分比的形式定义圆角的形状
*值1表示圆角水平方向半径，值2表示圆角垂直方向半径
*值2可以省略，默认沿用值1。
*/
border-top-left-radius：值1 值2

/*写法2
*如果提供全部的四个参数，那么将按照上左 、上右 、下右 、下左  的顺序作用于元素的四个角
*如果提供三个参数，那么第一个参数将作用于元素的左上角，第二个参数将作用于元素的右上角和左下角，第三个参数将作用于元素的右下角 
*如果提供两个参数，那么第一个参数将作用于元素的左上角和右下角，第二个参数将作用于元素的右上角和左下角 ；
*如果只提供一个参数，那么该参数将同时作用于元素的四个角。
*/
border: 值1/值2 值1/值2 值1/值2 值1/值2
```

### box-sizing：设置盒子模型大小

元素的实际宽度或高度取决于元素内容区、内边距以及边框的大小。因此，我们在为元素布局时还需要考虑元素的内边距和边框属性所占的页面空间。

正是由于上述原因，当为页面元素设置宽度和高度时，元素的实际大小比设置的要大。

为此 CSS3 中添加了 box-sizing 属性来改变默认的盒子模型，通过 box-sizing 属性可以<font color='red'>将元素的内边距和外边距在元素内容区内绘制</font>，以使元素呈现的宽度和高度与设置的宽度和高度相同。

`box-sizing`属性可选值：
值|描述
---|---
content-box| 默认值，元素的实际宽度或高度等于元素内容区的宽度或高度、内边距和边框的和
border-box| 在元素的内容区内绘制内边距或边框，内边距或边框不会影响元素的实际宽度或高度
inherit |从父元素继承 box-sizing 属性的值。

## CSS属性：布局

### 可见性(visibility)

用来设置元素是否可见

值 |描述
---|---
visible |默认值，表示元素是可见的
hidden| 隐藏元素
collapse |主要用来隐藏表格的行和列，隐藏的行或列所占的空间可以被其他表格内容使用；如果在其他元素上使用，其效果等同于“hidden”
inherit |从父元素继承 visibility 属性的值

### 显示类型(display)

用来控制元素的布局，设置元素是否显示以及如何显示

根据元素类型的不同，每个元素都有一个默认的 display 属性值，例如`<div>`默认的 display 属性值为 block（块级元素），而`<span>`默认的 display 属性值为 inline（行内元素）。

可以手动将元素的 display 属性转换为其它值。

display 属性的可选值如下：

值|描述
---|---
none| 隐藏元素
block |将元素设置为块级元素
inline| 将元素设置为内联元素
list-item| 将元素设置为列表项目
inline-block |将元素设置为行内块元素
table |将元素设置为块元素级的表格（类似`<table>`）
inline-table |将元素设置为内联元素级的表格（类似`<table>`）
table-caption| 将元素设置为表格的标题（类似`<caption>`）
table-cell |将元素设置为表格的单元格（类似`<td>`和`<th>`）
table-row |将元素设置为表格的行（类似`<tr>`）
table-row-group| 将元素设置为表格的内容部分（类似`<tbody>`）
table-column |将元素设置为表格的列（类似`<col>`）
table-column-group |将元素设置为表格中一个或多个列的分组（类似`<colgroup>`）
table-header-group |将元素设置为表格的头部（类似`<thead>`）
table-footer-group |将元素设置为表格的脚（类似`<tfoot>`）
inline-flex| CSS3 中新增的属性值，表示将对象设置为内联元素级的弹性伸缩盒（伸缩盒的最新版本）
run-in |根据上下文来决定将元素设置为块级元素或内联元素
inherit |从父元素继承 display 属性的值

>伸缩盒子（弹性盒子）是 CSS3 中一种新的布局模式，引入伸缩盒子的目的是提供一种更加有效的方式来对页面中的元素进行排列、对齐和分配空间，当页面需要适应不同的屏幕大小以及设备类型时这种布局方式能够确保元素拥有恰当尺寸和位置。

### 浮动(float)

浮动可以使一个元素脱离自己原本的位置，并在父元素的内容区中向左或向右移动，直到碰到父元素内容区的边界或者其它浮动元素为止。

`float` 属性有三个可选值，如下表所示：

值| 描述
---|---
left| 元素向左浮动
right| 元素向右浮动
none |默认值，元素不浮动
inherit| 从父元素继承 float 属性的值

### 定位(position)

设置元素在页面中的位置，`position` 属性有 5 个可选值，分别对应 5 种不同的定位方式

#### static

默认值，静态定位，表示没有定位，元素会按照正常的位置显示，此时 top、bottom、left 和 right 4 个定位属性也不会被应用。

#### relative

相对定位就是元素相对于自己默认的位置来进行位置上的调整。

可以通过 top、bottom、left 和 right 四个属性的组合来设置元素相对于默认位置在不同方向上的偏移量。

![位置属性演示](%E4%BD%8D%E7%BD%AE%E5%B1%9E%E6%80%A7%E6%BC%94%E7%A4%BA.gif)


```css
div.static {
            position: relative;
            top: 50px;
            left: 20px;
        }
```

#### absolute 绝对定位

绝对定位就是元素相对于第一个非静态定位（static）的父级元素进行定位，如果找不到符合条件的父级元素则会相对与浏览器窗口来进行定位。

同样可以使用 top、bottom、left 和 right 四个属性来设置元素相对于父元素或浏览器窗口不同方向上的偏移量。

![绝对定位](%E7%BB%9D%E5%AF%B9%E5%AE%9A%E4%BD%8D.gif)

使用绝对定位的元素会脱离原来的位置，不再占用网页上的空间。与相对定位相同，使用绝对定位的元素同样会与页面中的其它元素发声重叠，另外使用绝对定位的元素可以有外边距，并且外边距不会与其它元素的外边距发生重叠。

#### fixed 固定定位

固定定位就是将元素相对于浏览器窗口进行定位，使用固定定位的元素不会因为浏览器窗口的滚动而移动，就像是固定在了页面上一样
