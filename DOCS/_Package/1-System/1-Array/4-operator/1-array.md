---
layout: default

grand_parent: Array Class
parent: Operator
has_children: false
title: Array[ ] Operator
nav_order: 1
permalink: /package/system/array/operator/array
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">An operator that accesses the elements of an Array in an array format.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var obj = arr[ <b>indx</b> ]</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a reference to the element specified by <b>indx</b>. If no corresponding element is found for <b>indx</b>, a reference pointing to NULL is returned and the number of elements is expanded.</td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td><b>indx</b></td>
    <td>Subscript that specifies the element position of a number or string.<br><br>If you specify a number for indx, it indicates the same element as the string with the same value. For example, arr [10] and arr ["10"] have the same meaning.<br><br>When you specify a number for indx, you can specify a value between 0 and 2147483646.</td>
  </tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var arr = new Array("test1", "test2", "test3", "test4");
print(arr[2], "\n");
arr["aa"] = "aaaa";
print(arr["aa"], "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>
