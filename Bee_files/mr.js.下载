// 加载进度条
document.onreadystatechange=function(){
	if(document.readyState="complete"){
		$(".loading").fadeOut();
	}
}

// $(function(){
// 	setInterval(function(){
// 		$(".loading").fadeOut();
// 	},1000)
// })
// 


// //回到顶部按钮
$(function(){
//根据滚动距离判断按钮是否显示或隐藏
$(window).scroll(function(){
if($(this).scrollTop()>50){
	$("#back-to-top").fadeIn(100);
}
else{
	$("#back-to-top").fadeOut(100);
}
});
//实现点击滚动回到顶部
$("#back-to-top").click(function(){
	$("html,body").animate({scrollTop:0},50);
	return false;
})
})

window.onload = function(){
	showTime();
}
function checkTime(i){
	if(i<10){
		i = "0"+i;
		return i;
	}else{
		return i;
	}
}
function showTime(){
	var myData = new Date();  //获取系统时间
	var myYear = myData.getFullYear(); //获取年份
	var myMonth = myData.getMonth()+1; //获取月份 +1因为月份是从0开始
	var myDate = myData.getDate();     //获取日
	var myDay = myData.getDay();  	   //获取日期
	var myHours = myData.getHours();   //获取时
	var myMinutes = myData.getMinutes();  //获取分
	var mySeconds = myData.getSeconds();	 //获取秒
	myMinutes = checkTime(myMinutes);
	mySeconds = checkTime(mySeconds);
	var weekday=new Array(7)
    weekday[0]="星期日"
    weekday[1]="星期一"
    weekday[2]="星期二"
    weekday[3]="星期三"
    weekday[4]="星期四"
    weekday[5]="星期五"
    weekday[6]="星期六"
	document.getElementById("time").innerHTML = myYear+"年"+myMonth+"月"+myDate+"日"+"  "+ weekday[myDay]+"  "+myHours+":"+myMinutes+":"+mySeconds;
	setTimeout(showTime,500);

}