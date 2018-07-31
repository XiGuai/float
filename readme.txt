<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>浮动</title>
	<style>
	/* **浮动**
	让盒子从普通流中**浮**起来,
	主要作用让多个块级盒子一行显示。（让块级元素排列一行并没有间距）
	浮动元素不会占据父级盒子的边框和内边距
	*特点：
	浮：加了浮动的盒子**是浮起来**的，漂浮在其他标准流盒子的上面。 
	（文字不能占据浮动盒子的位置）
	漏：加了浮动的盒子**是不占位置的**，它原来的位置**漏给了标准流的盒子**。
	特：**特别注意**：浮动元素会改变display属性， 
	 类似把块级元素转换为了行内块，但是元素之间没有空白缝隙
	 **清除浮动：主要为了解决父级元素因为子级浮动引起内部高度为0的问题。给父级清除浮动之后
	 父级就会根据浮动的子盒子自动检测高度。父级有了高度，就不会影响下面的标准流了（当不适合设置父级高度时，由子级撑开盒子，但浮动的盒子不占据位置父级高度就变成了零）
	 ** 嵌套块元素垂直外边距的合并（塌陷）（设置子盒子margin父盒子和子盒子一起落下）
	对于两个嵌套关系的块元素，如果父元素没有上内边距及边框；父元素的上外边距会与子元素的上
	外边距发生合并合并后的外边距为两者中的较大者
	*行内元素：只能容纳文本或其它行内元素；一行可以容纳多个标签；宽高内外边距不可以设置；
	（大小为内容大小）（a标签可以包含块级元素，不能包含a标签）；（a、span、input、em-
	i、strong-b、del-s、ins-u、）
	 */
		.box {
			width: 300px;
			background-color: pink;
			overflow: hidden;	
			}
		.top {
			width: 100px;
			height: 100px;
			background-color: green;
			float: left;
		}
		.buttom {
			width: 200px;
			height: 200px;
			background-color: blue;
			float: right;
		}


	</style>
</head>
<body>
	<div class="box">
		<div class="top"></div>
		<div class="buttom"></div>
	</div>
	
</body>
</html>