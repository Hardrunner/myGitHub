<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
	<title></title>
	<style type="text/css">
		.container{display: flex;width: 500px;height: 400px;background-color: pink;margin: 10px;}
		.item{margin: 5px;width: 50px;text-align: center;background-color: skyblue;height:33px;line-height: 33px;}
		/*改为列排列时居左变为居上，居右变为居下左右居中变为上下居中*/
		/*.container{flex-flow: column;}*/
		.star{justify-content: flex-start;}
		.end{justify-content: flex-end;}
		.center{justify-content: center;}
		.between{justify-content: space-between;}
		.around{justify-content: space-around;}
	</style>
</head>
<body>
<!-- 所有子元素靠前排列 -->
<div class="container star">
	<div class="item">1</div>
	<div class="item">2</div>
	<div class="item">3</div>
</div>
<!-- 所有子元素靠后排列 -->
<div class="container end">
	<div class="item">1</div>
	<div class="item">2</div>
	<div class="item">3</div>
</div>
<!-- 居中对齐即剩余平分到父元素左右（或上下）就像父元素两侧的 padding-->
<div class="container center">
	<div class="item">1</div>
	<div class="item">2</div>
	<div class="item">3</div>
</div>
<!-- 剩余平分到子元素右侧 （或者下侧（列排列）） -->
<div class="container between">
	<div class="item">1</div>
	<div class="item">2</div>
	<div class="item">3</div>
</div>
<!-- 剩余平分到子元素左右（或者上下（列排列时）） -->
<div class="container around">
	<div class="item">1</div>
	<div class="item">2</div>
	<div class="item">3</div>
</div>
</body>
</html>
