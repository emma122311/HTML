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
1.判斷 ID 等於 ""
if (document.getElementById('test1').value == '') 
{
	alert('數值請勿為空');
}
2.同時判斷(條件1),（）條件2）不等於""
if (num1 !=='' && num2 !=='') 
{
　	num3.value =parseInt(num1)+parseInt(num2);
}
// 空值 = ""
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
js onkeyup 事件
```
<input type="text" onkeyup="myFunction()">
  //onkeyup 事件會在鍵盤被鬆開時發生。
```
js parseInt() 函数
```
parseInt() 函数可解析一个字符串，并返回一个整数。
 //num3.value =parseInt(num1)+parseInt(num2);

```
js 修改和獲取p標籤裡面的內容
```
 function test()
    {
        var num = document.getElementById("p");
        alert(num.innerHTML);
        num.innerHTML= "google coding"; 
    }
  //document.getElementById("p1").innerHTML = "google coding";
  function test2()
    {
        var num = document.getElementById("p2");
        alert(num.innerText);
        num.innerText= "knowledge"; 
    }
    
  //JavaScript 的 innerHTML 與 innerText 看似類似，但其實有很大的差異，
  //對大多數設計師來說 innerHTML 應該比較熟悉，
  //他是用來取得 HTML 元素或寫入字串到 HTML 網頁的語法，且 innerHTML 是 W3C 規定的標準寫法，
  // innerText 則是除了可以用來取得 HTML 元素之外，還會把元素的 HTML 標籤去除掉，
  // innerText 並非 W3C 所規定的標準寫法，而且僅適用於 IE 瀏覽器，這點非常重要。

```
JS 判斷是否為整數
```
<input type='text' onkeyup="value=value.replace(/^(0+)|[^\d]+/g,'')">
   //输入框只能输入正整数，输入同时禁止了以0开始的数字输入，防止被转化为其他进制的数值。
<input type="text" onkeyup="value=value.replace(/[^\-?\d.]/g,'')" /> //限制文本框只能输入正数，负数，小数
<input type="text" onkeyup="value=value.replace(/[^\d.]/g,'')" />  //限制文本框只能输入正数，小数

//onkeyup:事件會在鍵盤被鬆開時發生。
```
js 判斷輸入是否為數字
```
isNaN(numValue)
 EXP: if (isNaN(i) == false && isNaN(j) == false && i != ""  && j != "") 
 //判斷是否為數字//判斷是否為空值*/
```
Js isNAN()函數用於檢查其參數是否 是非數字值
```
  isNaN(x)
  isNaN(NaN) == true
  isNaN("hi") == true
  isNaN(undefined) == true
  isNaN(10) == false
  isNaN("10") == false
  //如果x是特殊的非數字值NAN(或者能被轉換為這樣的值),返回的值就是true。如果x是其他值,則返回false。
  //參考網址：https://coder.tw/?p=7435
```
 js input min屬性
 ```
 數量 (在1和5之間):
  <input type="number" name="quantity" min="1" max="5"><br>
  min 屬性規定 <input> 元素的最小值。
  //提示：min 屬性與 max 屬性配合使用，可創建合法值範圍。
  //注意：max 和 min 屬性適用於以下 input 類型：number、range、date、datetime、datetime-local、month、time 和 week。
 ```
 Js 每隔一秒就執行
```
setTimeout("test()",1000);
```

