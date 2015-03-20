# project-02-a-Kriti
<html>
<body>

<head>
<style type="text/css">
body
{
background-color:#FFCCFF;
}
</style>
</head>


<head>
<table width=100% height="300" border="0">
<tr>
<td colspan="10" style="background-color:#CCCCFF;">
<h1>
<font face="arial" color="blue">
CALCULATING PRODUCTIVITY RATING INDEX
<font/>
</h1>
</td>
</tr>
<table/>
<head/>


<p>
<font size="5" face="arial" color="blue">
Enter the Expected or Actual Yield
<font/>
</p>
<input  id="dem" type="number">
<p>
<font size="5" face="arial" color="blue">
Enter the Standard Yield
<font/>
</p>

<input id="nex" type="number" >
<br/>
<button type="button" onclick="function1()">Calculate PRI</button>
<p id="result"></p>
<button type="button" onclick="function2()">Check</button>
<p id="final"></p>



<script>
var r;
function function1()
{
 var e=document.getElementById("dem").value;
 var s=document.getElementById("nex").value;
 r=e*100/s;
 document.getElementById("result").innerHTML=r;
}
</script>



<script>
function function2()
{
 var t=document.getElementById("final").value;
 var k;
 if(t<20)
{ 
 k="N";
}
else if(t>20 && t<40)
{
 k="S3";
}
else if(t>40 && t<80)
{
 k="S2";
}
else
{
 k="S1";
}
document.getElementById("result").innerHTML=k; 
}
</script>

</body>
</html>
