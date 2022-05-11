---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.Concat Method
nav_order: 4
permalink: /package/system/string/methods/concat
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Concatenates the string specified in the argument to the original string.<br>This method updates the value of the String object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str.Concat( <b>text_1</b> [, <b>text_2</b> [, … ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Concatenated string</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>text_n</b></td>
    <td>String to concatenate<br>If multiple specifications are specified, all will be concatenated.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new String("ABC");
print(str.Concat("DEF", "GHI"), "\n");
print(str, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>