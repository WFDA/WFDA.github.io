<html>
 <head>
	<title>下拉菜单</title>
	<style type="text/css">
	 	 *{
	 	 	padding: 0px;margin: 0px;}
		 ul{
		 	list-style-type: none;

		 }
		 li{
		 	cursor: pointer;
		 }
		 .menu{
		 	line-height: 40px;
		 	width: 800px;
		 	margin: 0 auto;

		 }
		 .menu>li{  /* 子代选择器  */
		 	float: left;
		 	padding: 0px 0px;
		 	background: rgb(0,161,214);
		 	width: 120px;
		 	text-align: center;		 	 
		 }
		 .sub{
		 	display: none;
		 }
		 .sub li{
		 	padding: 0px 0px;
		 	border-bottom: 1px solid #fff; /* 1px的分割线 颜色#fff */
		 }
	</style>
	<script type="text/javascript">
	
		/*function show(str){
				var KC=document.getElementById('KC');
				KC.style.display="block";
		}*/
		function show(str) {
			// body...
			
			return document.getElementById(str).style.display="block";
				
		}
			
			
		
		/*function hide(str){
				var KC=document.getElementById('KC');		
				KC.style.display="none";
		}*/
		function hide(str) {
			// body...
				
				return document.getElementById(str).style.display="none";	
				
		}	
	</script>
 </head>
 <body>
 	<ul class="menu">
 	<li>首页</li>
 	<li onmouseover="show('KC')" onmouseout="hide('KC')"> 
 		课程
 		<ul class="sub" id="KC"> 
 			<li>JavaScript</li>
 			<li>Css</li>
 			<li>Html</li>
 			<li>Jsp</li>
 		</ul>
 	</li>
 	<li  onmouseover="show('XX')" onmouseout="hide('XX')">
 		学习
 		<ul class="sub" id="XX">
 			<li>Java学习</li>
 			<li>Css 学习</li>
 			<li>Html学习</li>
 			<li>Jsp 学习</li>
 		</ul>
 	</li>
 	<li onmouseover="show('AL')" onmouseout="hide('AL')">
 		案例
 		<ul class="sub" id="AL">
 			<li>Java案例</li>
 			<li>Css 案例</li>
 			<li>Html案例</li>
 			<li>Jsp 案例</li>
 		</ul>
 	</li>
 	<li>关于</li> 
 	</ul>
 	
 </body>
</html>
