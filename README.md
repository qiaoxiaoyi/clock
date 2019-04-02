# clock
Js   clock
<html

<head>

<meta charset="UTF-8">

<title>网页时钟</title>

<script type="text/javascript">

function displayTime()
{
//1.获取div元素

var timeDiv=document.getElementById("timeDiv");

//2.获取系统当前时间

var nowTime=new Date();
var strNowTime=nowTime.toLocaleString();

//3.将系统时间设置到div元素中

timeDiv.innerHTML=strNowTime;
}

//每隔1秒调用一次displayTime函数

function start(){
window.setInterval("displayTime()",1000)//单位是毫秒
}

</script>

</head>

<!--? body onload:当整个html页面加载完成后执行此函数? -->

<body onload="start();">

<div id="timeDiv">
</div>

</body>

</html>

