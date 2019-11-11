# HTML
提示框
```
alert('出現警示框');
```
一開視窗就執行
```
window.onload = welcome;
function welcome() 
{
	alert('歡迎光臨');
}
	//welcome 方選名稱
```
js 點擊觸發
```
 onclick="Show()"
 	//Show 方選名稱
```
js console.log 偵錯 （console.log）
```
function Show()
{
	console.log('123'); 
}
	//console.log(輸出)	
```
js Global Variable 全域變數與 Local Variable 區域變數  
```
var num = 1;
	//宣告全域變數(不在方選內)
```
js 宣告方選（方選名字不重複）
```
function text()
{
	alert('出現警示框');
}
	//test(名稱)
```
js  if , else if ,else 判斷式
```
function test()
{
	if(條件式)		//如果
	{
		
	}
	else if(條件式)	
	{
	
	}
	else(條件式)
	{
	}
}

```

js 使用for迴圈
```
for (语句 1; 语句 2; 语句 3) 
{
     要执行的代码块
}
	//例如：for(i=1;i<=10;i++){}  輸出後會在console裡面出現1~10

```
onchange Event
```
function ShowStr(x)
{
	var Str=document.getElementById(x).value;
	alert(Str);
}

	//請隨意輸入幾個文字：<input type="text" id="Str" onchange="ShowStr(this.id)">
	//當輸入完文字滑鼠移開文字欄位就會觸發onchange Event
```
九九乘法
```
for(i = 1;i<=10;i++)
{
	console.log("2" +"x"+ i + "=" + 2*i);
}
	//利用for迴圈使變數產生數字,輸出後會產生1~9
	//再使兩個變數相乘
	//輸出結果（2x1=2 ... 2x10=20）
```
js 獲取 input 的 value
```
 var name = document.getElementById("name").value;
 	alert(name);
	//var name = value
	//document.getElementById("name")=id
```
js 改變input的 value
```
<input type="text"  id="test1"  value="初始文字內容" > X
<input type="text"  id="test2" >
<button type="button" onclick="test()"> 等於 </button>
<input type="text"  id="t3"  value="更改文字內容">
<script>
	function test()
	{
		var t1 = document.getElementById("test1").value;
		var t2 = document.getElementById("test2").value;
		
		if(t1!='' && t2!='')
		{		
			t3.value = t1*t2 ;
		}
		else
		{
			alert('數值不能為空');
		}
		//!='' 不等於空值
		//t1*t2 = 修改的文字內容
	}
</script>
```
js 判斷 input 空值
```
if (document.getElementById('test1').value == '') 
{
　alert('數值請勿為空');
}
```
js 判斷 1~100 為(2)的倍數
```
for (i=1;i<=100;i++)
　{  
　　if (i%2 == 0)
　　{
　　　console.log(i);
　　}
　}
```
