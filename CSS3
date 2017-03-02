#样式

##边框

###圆角效果
`border-radius:5px 5px 5px 5px;`(左上 右上 右下 左下)

![](http://img.mukewang.com/52e216d2000195ef01110111.jpg)

`width:100px;height:100px;`

`border-radius:50px;`(为长宽的一半，圆形)

***
###阴影

![](http://img.mukewang.com/54292d620001ffb107080250.jpg)
box-shadow: X轴偏移量 Y轴偏移量 [阴影模糊半径] [阴影扩展半径] [阴影颜色] [投影方式];
***
####外阴影
`.box_shadow{
  box-shadow:4px 2px 6px #333333; 
}`
![](http://img.mukewang.com/52e21c9000013c8f01180117.jpg)
####内阴影
`.box_shadow{
  box-shadow:4px 2px 6px #333333 inset; 
}`
![](http://img.mukewang.com/54292b990001ebea01290115.jpg)

####多重阴影
`.box_shadow{
    box-shadow:4px 2px 6px #f00, -4px -2px 6px #000, 0px 0px 12px 5px #33CC00 inset;
}`
![](http://img.mukewang.com/52e21d210001356d01170116.jpg)
***

###边框图片

![](http://img.mukewang.com/52e2201a0001b1e004720260.jpg)

边框图片(每个菱形长宽均为70)

![](http://img.mukewang.com/52e21fea000127e802100210.jpg)

样式

`border-image:url(borderimg.png) 70 repeat;`(重复)

![](http://img.mukewang.com/52e220780001091a03530354.jpg)

`border-image:url(borderimg.png) 70 round;`(铺满，边框效果会拉伸或者压缩)

![](http://img.mukewang.com/52e2216700014c4103190312.jpg)

`border-image:url(borderimg.png) 70 stretch`(拉伸不重复)

![](http://img.mukewang.com/52e2218d0001d45403530366.jpg)

##颜色

###RGBA
`color：rgba(R,G,B,A)`RGB三原色，取值为0-255或0.0%-100.0%，A为透明度取值为0-1。
***
###渐变
![](http://img.mukewang.com/54b72b2e0001500103790158.jpg)

![](http://img.mukewang.com/542a25da00017e9406980223.jpg)

`background-image:linear-gradient(to left, red, orange,yellow,green,blue,indigo,violet);`

![](http://img.mukewang.com/54b72c080001611c04230192.jpg)
***
##文字和字体
###文字溢出控制text-overflow和换行word-warp
![](http://img.mukewang.com/53070cc00001a5bc06000200.jpg)

![](http://img.mukewang.com/53070cf700018a2b06000200.jpg)
text-overflow只是用来说明文字溢出时用什么方式显示，要实现溢出时产生省略号的效果，还须定义强制文本在一行内显示（white-space:nowrap）及溢出内容为隐藏（overflow:hidden），只有这样才能实现溢出文本显示省略号的效果，代码如下

`text-overflow:ellipsis; 
overflow:hidden; 
white-space:nowrap; `
***
###嵌入字体
`@font-face {
    font-family : 字体名称;
    src : 字体文件在服务器上的相对或绝对路径;
}`

这样设置之后，就可以像使用普通字体一样在（font-*）中设置字体样式。

`p {
    font-size :12px;
    font-family : "My Font";
    /*必须项，设置@font-face中font-family同样的值*/
}`
***
###文本阴影text-shadow
语法：

`text-shadow: X-Offset Y-Offset blur color;`

X-Offset：表示阴影的水平偏移距离，其值为正值时阴影向右偏移，反之向左偏移；      

Y-Offset：是指阴影的垂直偏移距离，如果其值是正值时，阴影向下偏移，反之向上偏移；

Blur：是指阴影的模糊程度，其值不能是负值，如果值越大，阴影越模糊，反之阴影越清晰，如果不需要阴影模糊可以将Blur值设置为0；

Color：是指阴影的颜色，其可以使用rgba色。
***
##背景
###背景起始位置background-origin
`background-origin ： border-box | padding-box | content-box;`(边框 、 内边距（默认值）、内容区域)


![](http://img.mukewang.com/531003de0001166903660166.jpg)

***
###背景裁剪background-clip
语法：

`background-clip ： border-box | padding-box | content-box | no-clip`(边框、内填充、内容区域、不裁剪)

![](http://img.mukewang.com/5310065d0001c95103660166.jpg)

***
###背景图大小background-size
语法：

`background-size: auto | <长度值> | <百分比> | cover | contain`

取值说明：

1、auto：默认值，不改变背景图片的原始高度和宽度；

2、<长度值>：成对出现如200px 50px，将背景图片宽高依次设置为前面两个值，当设置一个值时，将其作为图片宽度值来等比缩放；

3、<百分比>：0％~100％之间的任何值，将背景图片宽高依次设置为所在元素宽高乘以前面百分比得出的数值，当设置一个值时同上；

4、cover：顾名思义为覆盖，即将背景图片等比缩放以填满整个容器；

5、contain：容纳，即将背景图片等比缩放至某一边紧贴容器边缘为止。

###多重背景multiple backgrounds

多重背景，也就是CSS2里background的属性外加origin、clip和size组成的新background的多次叠加，缩写时为用逗号隔开的每组值；用分解写法时，如果有多个背景图片，而其他属性只有一个（例如background-repeat只有一个），表明所有背景图片应用该属性值。

`background-repeat : repeat1,repeat2,...,repeatN;
backround-position : position1,position2,...,positionN;
background-size : size1,size2,...,sizeN;
background-attachment : attachment1,attachment2,...,attachmentN;
background-clip : clip1,clip2,...,clipN;
background-origin : origin1,origin2,...,originN;
background-color : color;`

`background-image: url(http://img.mukewang.com/54cf2365000140e600740095.jpg),
                      url(http://img.mukewang.com/54cf238a0001728d00740095.jpg),
                      url(http://img.mukewang.com/54cf23b60001fd9700740096.jpg);
    background-position: left top, 100px 0, 200px 0;
    background-repeat: no-repeat, no-repeat, no-repeat;`
![](http://img.mukewang.com/54cf289200013de502790094.jpg)

********
#选择器

##属性选择器
![](http://img.mukewang.com/56653eba0001b07004610215.jpg)

实例展示：

html代码：

`<a href="xxx.pdf">我链接的是PDF文件</a>
<a href="#" class="icon">我类名是icon</a>
<a href="#" title="我的title是more">我的title是more</a>`

css代码  

`a[class^=icon]{
  background: green;
  color:#fff;
}
a[href$=pdf]{
  background: orange;
  color: #fff;
}
a[title*=more]{
  background: blue;
  color: #fff;
}`

效果

![](http://img.mukewang.com/53202e050001c07e03820068.jpg)

##结构性伪类选择器
###root

:root”选择器等同于<html>元素，简单点说：

:root{background:orange}

html {background:orange;}

效果相同
***
###not

:not选择器称为否定选择器，和jQuery中的:not选择器一模一样，可以选择除某个元素之外的所有元素。


就拿form元素来说，比如说你想给表单中除submit按钮之外的input元素添加红色边框，CSS代码可以写成：
`form {
  width: 200px;
  margin: 20px auto;
}
div {
  margin-bottom: 20px;
}
input:not([type="submit"]){
  border:1px solid red;
}`
相关HTML代码：
<form action="#">
 <div>
    <label for="name">Text Input:</label>
    <input type="text" name="name" id="name" placeholder="John Smith" />
  </div>
  <div>
    <label for="name">Password Input:</label>
    <input type="text" name="name" id="name" placeholder="John Smith" />
  </div>
  <div>
    <input type="submit" value="Submit" />
  </div>
</form>​
结果：

![](http://img.mukewang.com/531eb2ca00014b5002370177.jpg)

***
###empty
:empty选择器表示的就是空。用来选择没有任何内容的元素，这里没有内容指的是一点内容都没有，哪怕是一个空格。

HTML代码：

`<p>我是一个段落</p>`

`<p> </p>`

`<p></p>`

​
CSS代码：

`p{	
 background: orange;
 min-height: 30px;
}
p:empty {
  display: none;
}`​
演示结果：

![](http://img.mukewang.com/531eb55b0001d7d401580126.jpg)
***
###target

:target选择器称为目标选择器，用来匹配文档(页面)的url的某个标志符的目标元素。
