---
layout: default

grand_parent: Byte Array Class
parent: Methods
has_children: false
title: ByteArray.ToUString Method
nav_order: 4
permalink: /package/system/bytearray/methods/toustring
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the data stored in the ByteArray object as a Unicode string. If a null character appears in the data, the data after that is ignored.<br><br><small>Added since Ver.5.0.1</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ustr = barr.ToUString ()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">UString type string</td>
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
    <td colspan="2"><code><pre>var f = fs.OpenDialog (" Read File ", "Unicode Text (* .txt) = * .txt", "txt", "");
var b = f.ReadBinary ();
var ustr = b.ToUString ();</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





