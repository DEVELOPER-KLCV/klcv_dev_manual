---
layout: default

grand_parent: UString Class
parent: Methods
has_children: false
title: UString.Substring Method
nav_order: 12
permalink: /package/system/ustring/methods/substring
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Cut out a part of the character string.<br><br>This method cuts out the character string without being aware of the character type of the target character string. Use the <br><a href="/method/str/mid">mid</a> function to cut out a character string that contains double - byte characters in the target character string.<br><br>The difference with <a href="/package/system/string/methods/slice">Slice</a> method<br>The smaller value of <b>start</b> and <b>end</b> is the start position of the character string to be acquired. (Substring (0, 3) and Substring (3, 0) have the same result)<br>If a negative value is specified for the argument, it is replaced with 0.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str.Substring( <b>start</b>, <b>end</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Cut out character string</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>start</b></td>
    <td>Leading position to cut out<br>Specify a number starting from 0</td>
  </tr>
  <tr>
    <td>integer <b>end</b></td>
    <td>End position to cut out (cut out to the character before the specified position)<br>Specify a number starting from 0</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new UString("abcdefghi");
print(str.Substring(1, 2), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/ustring/methods/slice">Slice</a> method</td>
  </tr>
</table>