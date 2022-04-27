---
layout: default

parent: System Functions

title: encodeURL
nav_order: 6
permalink: /method/system/encodeURL
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">URL-encode the string. <br><small> Added since Mobile Ver.2.0.0</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = encodeURL  (<b>str</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns an encoded string.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>str</b></td>
    <td>Specify the character string to decode.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var name = " Biz Browser & Designer ";
var value = "Biz / Browser & Designer";
var url = "http: // server / app1? name =" + encodeURL (name) + "& value =" + encodeURL (value);
print (url, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/statistical/decodeURL">decodeURL</a> function</td>
  </tr>
</table>





