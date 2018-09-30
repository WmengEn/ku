#ku
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>HTML5+CSS3制作日历图标</title>
	<style type="text/css">
	*{
		margin:0;
		padding:0;	}
		div{
			width:500px;
			height:500px;
			margin:100px auto;
		}
		time.icon{
			/*改变icon size*/
			font-size: 16px;
			display: block;
			/*相对定位*/
			position:relative;
			width:112px;
			height:112px;
			background-color:#fff;
			border-radius:10px;
			box-shadow:0 1px 0 #bdbdbd, 0 2px 0 #fff, 0 3px 0 #bdbdbd, 0 4px 0 #fff, 0 5px 0 #bdbdbd, 0 0 0 1px #bdbdbd;
			overflow:hidden;
		}
		/*基础样式*/
		time.icon*{
			display: block;
			width:100%;
			font-size: 16px;
			font-weight: bold;
			font-style: normal;
			text-align: center;
		}
		/*定义月份样式*/
		time.icon strong{
			position:absolute;
			top:0;
			padding:6px 12px;
			color:#fff;
			background-color:#fd9f1b;
			border-bottom:1px dashed #f37302;
			box-shadow:0 2px 0 #fd9f1b;
		}
		/*星期放在图标底部*/
		time.icon em{
			position:absolute;
			bottom:5px;
			left:18px;
			color:#000000;
		}
		/*放大定位日期*/
		time.icon span{
			font-size: 50px;
			/*两个数字之间的距离（字间距）*/
			letter-spacing: -2px;
			/*padding-top:15px;*/
			color:#f90c0c;
			position:absolute;
			top:30px;
			left:26px;
			/*给文字加投影*/
			text-shadow:1px 2px 0px #ccc;
		}




	</style>
</head>
<body>
	<!-- <time>2018-09-29T12:44:00Z</time>
	<time datetime="2018-09-29T12:44:00+08:00">20:45pm,Saturday September 29<sup>th</sup>,2018</time> -->
	<div>
	<time datetime="2018-09-29" class="icon">
		<em>Saturday</em>
		<strong>September</strong>
		<span>29</span>
	</time>
	</div>
</body>
</html>
