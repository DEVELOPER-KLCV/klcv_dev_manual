---
layout: default

grand_parent: Array
parent: Method
has_children: false
title: Array constructor
nav_order: 1
permalink: /package/system/array/method/constructor
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize the Array object.<br><br>If <b>item_n</b> is specified, <b>item_n</b> will be initialized as an array element.<br>If <b>len</b> is specified, it will be initialized as <b>len</b> empty elements.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var arr = new Array( [ <b>item_1</b> [, <b>item_2</b> [, … ] ] ] )<br>var arr = new Array( <b>len</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Array object</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>item_n</b></td>
    <td>Object to be an array element</td>
  </tr>
  <tr>
    <td>Integer <b>len</b></td>
    <td>Number of elements in the array</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var arr1 = new Array("test1", "test2", "test3");
var arr2 = new Array(3);
arr2[0] = "test1";
arr2[1] = "test2";
arr2[2] = "test3";
print(arr1.ToString(), "\n");
print(arr2.ToString(), "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



