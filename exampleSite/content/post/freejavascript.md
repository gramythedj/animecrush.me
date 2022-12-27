---
title: 'free javascripts testing'
date: 2022-12-26T06:20:00.001-08:00
draft: false
url: /2022/12/freejavascript.html
tags: 
- news
- anime
---





<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>quadratic2</title>
</head>
<body>
    <!--Script by hscripts.com-->
<!-- Free javascripts @ https://www.hscripts.com -->
<!-- Script by hscripts.com -->
<form name="qfrm">
    <table>
    <tr>
    <td><input type="text" name="av" id="av" size="3" onkeyup="isNumberKey(this.id)">x<sup>2</sup>+</td>
    <td><input type="text" name="bv" id="bv" size="3" onkeyup="isNumberKey(this.id)">x+</td>
    <td><input type="text" name="cv" id="cv" size="3" onkeyup="isNumberKey(this.id)"></td></tr>
    <tr rowspan="2"><td colspan="3" align="center"><input type="button" value="Calculate" onclick="quad()"></td></tr>
    </table>
    <table>
    <tr rowspan="2"><td colspan="3" align="center">Result</td></tr>
    <tr><td>Root 1<input type="text" name="r1" id="r1" size="10" readonly></td>
    <td>Root 2<input type="text" name="r2" id="r2" size="10" readonly></td></tr>
    </table>
    </form>

    

<script type="text/javascript">
function quad()
{
var a=document.getElementById("av").value;
var b=document.getElementById("bv").value;
var c=document.getElementById("cv").value;
var d=(Math.pow(b,2)-(4*a*c));
var x1=(-b + Math.sqrt(d)) / (2*a);
var x2=(-b - Math.sqrt(d)) / (2*a);
document.getElementById("r1").value=x1;
document.getElementById("r2").value=x2;
if(document.getElementById("r1").value == "NaN")
document.getElementById("r1").value="imag";
if(document.getElementById("r2").value == "NaN")
document.getElementById("r2").value="imag";
}
var check=true;
function isNumberKey(id)
{var no=eval('"'+id+'"');var number= document.getElementById(no).value;if(number.length==1){
check=true;}if(number.length>1){
var dd = number;
if(dd.substring(dd.length,(dd.length-1))=='-')
{
if(check)
{
check=false;
}
else
{
dd = dd.substring(0,(dd.length-1));
document.getElementById(no).value = dd;
}
}}if(!number.match(/^[0-9-]+$/) && number !=""){document.getElementById(id).value="";document.getElementById(id).focus();}else{
var dd = number;if(dd.substring(dd.length,(dd.length-1))=='-'){
if(check)
{
check=false;
}
else
{
document.getElementById(id).value="";
document.getElementById(id).focus();
}}
}
}
</script>
<!-- Script by hscripts.com -->


  
</body>
</html>