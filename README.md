# design_login

![Alt text](https://raw.githubusercontent.com/daimingyu/photos/master/login.gif)

## 一、前言

dribbble地址 : [Deepak Yadav - Sign Up and Login Animated](https://dribbble.com/shots/2311260-Day-1-Sign-Up-and-Login-Animated-Download-Template)


## 二、文件夹

* /font：一个Roboto-Light.ttf字体文件。
* /js：一个jquery.js库文件。
* /photos：一些icon和背景图片等。
* /index.html : 入口文件

## 三、重要代码

### 1.字体文件引入
```
@font-face{
	font-family:roboto-light;
	src:url(fonts/Roboto-Light.ttf);
}
```
### 2.placeholder字体颜色
```
::-webkit-input-placeholder {  /* WebKit browsers */
	color:#dddddd;
}
:-moz-placeholder { /* Mozilla Firefox 4 to 18 */ 
	color: red; 
} 
::-moz-placeholder { /* Mozilla Firefox 19+ */ 
	color: red; 
} 
:-ms-input-placeholder { /* Internet Explorer 10+ */ 
	color: red; 
} 
```
<font color="red">注意 : 使用时一定要将这几条规则放在对应input前</font>

### 3.图片下方有空白

如何解决div里面img图片下方有空白的问题 : 霞光一点 https://jingyan.baidu.com/article/7082dc1c69dc6fe40a89bdfe.html

### 4.width与min-width联合使用
这个div块宽度随着网页的大小变化，网页在全屏的时候div宽度也全屏，但是网页缩到无论怎么小的时候，div最小宽度也就720px。
```
div{
	min-width:720px;
	width:100%
}
```
