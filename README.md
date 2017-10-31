<!doctype html>
<html>
<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="chrome=1">
	<title>蓝色星空岛</title>

	<link rel="stylesheet" href="style.css">
	<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
	<script>
		fixScale = function(doc) {
			var addEvent = 'addEventListener',
			type = 'gesturestart',
			qsa = 'querySelectorAll',
			scales = [1, 1],
			meta = qsa in doc ? doc[qsa]('meta[name=viewport]') : [];
			function fix() {
				meta.content = 'width=device-width,minimum-scale=' + scales[0] + ',maximum-scale=' + scales[1];
				doc.removeEventListener(type, fix, true);
			}
			if ((meta = meta[meta.length - 1]) && addEvent in doc) {
				fix();
				scales = [.25, 1.6];
				doc[addEvent](type, fix, true);
			}
		};
	</script>


	<!--[if lt IE 9]>
	<script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
	<![endif]-->
</head>
<body>
	<div class="wrapper">
		<header >
			<h1 style="text-align:center;width:100%;">欢迎来到蓝色星空岛</h1>
			<p id="time" style="text-align:center;width:100%;margin-top:10px;">蓝色星空岛</p>
		</header>
		<section style="border-right: 1px solid #FFF;">
			<h3>PC端效果</h3>
			<p>自己平时写的一些小特效：</p>
			<ol id="pc_items">
				<!-- <li>黑客效果特效   <a href="../effects/黑客效果特效.html" target="_blank">点击查看</a></li>
				<li>citytest省市区选择器  <a href="../effects/citytest省市区选择器.html" target="_blank">点击查看</a></li>
				<li>上传图片压缩  <a href="../effects/上传图片压缩.html" target="_blank">点击查看</a></li>
				<li>两点之间距离并连线或画三角形  <a href="../effects/两点之间距离并连线或画三角形.html" target="_blank">点击查看</a></li>
				<li>取随机数  <a href="../effects/取随机数.html" target="_blank">点击查看</a></li>
				<li>在数组m中找出他们的组合加起来为和为n的几组排列  <a href="../effects/在数组m中找出他们的组合加起来为和为n的几组排列.html" target="_blank">点击查看</a></li>
				<li>拖动js  <a href="../effects/拖动js.html" target="_blank">点击查看</a></li>
				<li>数组去重  <a href="../effects/数组去重.html" target="_blank">点击查看</a></li>
				<li>自己写的日历  <a href="../effects/自己写的日历.html" target="_blank">点击查看</a></li>
				<li>获取年月日时分秒  <a href="../effects/获取年月日时分秒.html" target="_blank">点击查看</a></li>
				<li>菜单伸缩  <a href="../effects/菜单伸缩.html" target="_blank">点击查看</a></li>
				<li>输入中文输出拼音  <a href="../effects/输入中文输出拼音.html" target="_blank">点击查看</a></li>
				<li>逐字输出  <a href="../effects/逐字输出.html" target="_blank">点击查看</a></li>
				<li>焦点图  <a href="../effects/焦点图/焦点图.html" target="_blank">点击查看</a></li>
				<li>map选择省市区加输入详细地址定位  <a href="../effects/地图/map选择省市区加输入详细地址定位.html" target="_blank">点击查看</a></li>
				<li>3D旋转  <a href="../effects/3D旋转/3D旋转.html" target="_blank">点击查看</a></li>
				<li>获取浏览器窗口各个属性  <a href="../effects/获取浏览器窗口各个属性.html" target="_blank">点击查看</a></li>
				<li>h5上传预览  <a href="../effects/h5上传预览.html" target="_blank">点击查看</a></li>
				<li>时间选择控件  <a href="../effects/时间选择控件/index.html" target="_blank">点击查看</a></li>
				<li>json ajax  <a href="../effects/json/json.html" target="_blank">点击查看</a></li>
				<li>数组排序  <a href="../effects/排序.html" target="_blank">点击查看</a></li>
	            <li>获取url里面的参数  <a href="../effects/获取url里面的参数.html" target="_blank">点击查看</a></li>
				<li>网易云音乐轮播图  <a href="../effects/网易云音乐轮播图/网易云音乐轮播图.html" target="_blank">点击查看</a></li>
				<li>网易云音乐轮播图(代码精简版)  <a href="../effects/2017-10-27网易云音乐轮播图/index.html" target="_blank">点击查看</a></li> -->
			</ol>
			
		</section>
		<section>
			<h3>手机端效果（必须在手机端看）</h3>

			<p>自己平时写的一些小特效：</p>
			<ol id="phone_items">
				<!-- <li>手机三级联动城市选择特效   <a href="../effects/phone/手机三级联动城市选择特效/index.html" target="_blank">点击查看</a></li>
				<li>mobile移动端键盘   <a href="../effects/phone/mobile移动端键盘.html" target="_blank">点击查看</a></li>
				<li>移动端左滑动删除效果   <a href="../effects/phone/移动端左滑动删除效果.html" target="_blank">点击查看</a></li>
				<li>map2输入地址定位或者点击地图定位  <a href="../effects/地图/map2输入地址定位或者点击地图定位.html" target="_blank">点击查看</a></li> -->
			</ol>
			
		</section>
	</div>
	<footer>

		<p>The Pages &mdash; Theme by <a href="http://dlovel.com">蓝色星空岛</a></p>
	</footer>
	<!--[if !IE]><script>fixScale(document);</script><![endif]-->

	<script type="text/javascript">
		var t ;
		(function myTime(){
			var date = new Date();//获取年月日时分秒
			y=date.getYear()+1900;//获取年份
			ys=date.getFullYear();//获取年份
			ms=date.getMonth()+1;//获取月份
			d=date.getDate();//获取天数
			h=date.getHours();//获取小时
			m=date.getMinutes();//获取分钟
			s=date.getSeconds();//获取秒钟
			document.getElementById("time").innerHTML=ys+"-"+ms+"-"+d+"&nbsp;&nbsp;&nbsp;&nbsp;"+h+":"+m+":"+s;//显示年月日时分秒
			t = setTimeout(myTime,1000);//定时器
		})()

		//pc端
		var boxArrays = [
							["黑客效果特效","黑客效果特效.html"],
							["citytest省市区选择器","citytest省市区选择器.html"],
							["上传图片压缩","上传图片压缩.html"],
							["两点之间距离并连线或画三角形","两点之间距离并连线或画三角形.html"],
							["取随机数","取随机数.html"],
							["在数组m中找出他们的组合加起来为和为n的几组排列","在数组m中找出他们的组合加起来为和为n的几组排列.html"],
							["拖动js","拖动js.html"],
							["数组去重","数组去重.html"],
							["自己写的日历","自己写的日历.html"],
							["获取年月日时分秒","获取年月日时分秒.html"],
							["菜单伸缩","菜单伸缩.html"],
							["输入中文输出拼音","输入中文输出拼音.html"],
							["逐字输出","逐字输出.html"],
							["焦点图","焦点图/焦点图.html"],
							["map选择省市区加输入详细地址定位","地图/map选择省市区加输入详细地址定位.html"],
							["3D旋转","3D旋转/3D旋转.html"],
							["获取浏览器窗口各个属性","获取浏览器窗口各个属性.html"],
							["h5上传预览","h5上传预览.html"],
							["时间选择控件","时间选择控件/index.html"],
							["json ajax","json/json.html"],
							["数组排序","排序.html"],
							["获取url里面的参数","获取url里面的参数.html"],
							["网易云音乐轮播图","网易云音乐轮播图/网易云音乐轮播图.html"],
							["网易云音乐轮播图(代码精简版)","2017-10-27网易云音乐轮播图/index.html"]
						]
		var boxId = document.getElementById("pc_items"),
			htmls = "";

		for(var i=0,len=boxArrays.length;i<len;i++){
			htmls+='<li><a href="../effects/'+ boxArrays[i][1] +'" target="_blank">'+ boxArrays[i][0] +'</a></li>'
		}
		boxId.innerHTML=htmls

		//移动端
		var phoneArrays  =  [
								["手机三级联动城市选择特效","phone/手机三级联动城市选择特效/index.html"],
								["mobile移动端键盘","phone/mobile移动端键盘.html"],
								["移动端左滑动删除效果","phone/移动端左滑动删除效果.html"],
								["map2输入地址定位或者点击地图定位","地图/map2输入地址定位或者点击地图定位.html"]
							]
		var phoneId = document.getElementById("phone_items"),
			phone_htmls = "";

		for(var j=0,lens=phoneArrays.length;j<lens;j++){
			phone_htmls+='<li><a href="../effects/'+ phoneArrays[j][1] +'" target="_blank">'+ phoneArrays[j][0] +'</a></li>'
		}

		phoneId.innerHTML = phone_htmls

	</script>

</body>
</html>
