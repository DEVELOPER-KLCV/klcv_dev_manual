---
layout: default

grand_parent: Byte Array Class
parent: Methods
has_children: false
title: ByteArray.ToString Method
nav_order: 3
permalink: /package/system/bytearray/methods/tostring
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the data stored in the ByteArray object as a string. If a null character appears in the data, the data after that is ignored.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var str = barr.ToString ()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Converted string</td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var barr = new ByteArray (0x41, 0x42, 0x43);
print (barr.ToString (), "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



