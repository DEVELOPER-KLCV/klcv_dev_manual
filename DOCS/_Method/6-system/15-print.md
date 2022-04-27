---
layout: default

parent: System Functions

title: print
nav_order: 15
permalink: /method/system/print
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Display debug messages in Biz / Designer. Ignored except during debugging on Biz / Designer. <br> It has the same function as the <a href="/method/system/debugMessage">debugMessage</a> function.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">print( <b>msg_1 [, msg_2 [, msg_3 ... ] ] </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Object <b> msg_n</b></td>
    <td>Specify the object to display.<br> The object is converted to a string and displayed. <br>To start a new line at the end of a line, specify "￥ n" at the end.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = 100;
var s = "sample";
print (d, s, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/system/debugMessage">debugMessage</a> function.</td>
  </tr>
</table>





