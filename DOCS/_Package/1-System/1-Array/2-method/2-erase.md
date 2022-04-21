---
layout: default

grand_parent: Array Class
parent: Methods
has_children: false
title: Array.Erase method
nav_order: 2
permalink: /package/system/array/methods/erase
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Deletes the element at the specified position or all elements.<br>**<small>Added since Version 4.0.3</small>**<br>**<small>Added since Mobile Version 3.0.0</small>**</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">arr.Erase( [ <b>index</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td><b>index</b></td>
    <td>Specify the index that specifies the element you want to delete.<br>If <b>index</b> is a number, subsequent elements with the number as a subscript are padded forward.<br>If <b>index</b> is omitted, all elements will be deleted.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var arr = new Array("test1", "test2", "test3", "test4");
print(arr, "\n");
arr.Erase(2);
print(arr, "\n");
arr.Erase();
print(arr.Length, "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>