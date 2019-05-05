<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title>Math.random()</title>
</head>
<body>
<script>
    var arr=[]; //定义空数组
     function getRandom(m,n){
     	var digit=m+n-1;
     	for(var i=0; i<10;i++){
     		arr[i]=Math.floor(Math.random()*digit+m); //将随机数赋值给原空数组
     	}
     	return arr;

     }
     var random=getRandom(0,100);
     var descend=random.sort(function(a,b){return b-a}); //将得到的随机数组降序排列
     document.write(descend+"<br/>");
     document.write("这组数的最大值是"+arr[0]+","+"最小值是"+arr[9]);

</script>
</body>
</html>
