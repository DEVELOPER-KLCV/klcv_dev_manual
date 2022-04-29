---
layout: default

parent: 6. System Functions

title: debugMessage
nav_order: 3
permalink: /method/system/debugMessage
---



# {{ page.title }}   

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"> Display debug messages in Biz / Designer. Ignored except during debugging on Biz / Designer. <br> The abbreviation <a href="/method/statistical/print">print</a>  function is also available.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">debugMessage (<b>msg_1 [, msg_2 [, msg_3 ...]]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Object <b>msg_n</b></td>
    <td>Specifies the object to display. <br> The object is converted to a string and displayed. <br> To start a new line at the end of a line, specify "￥ n" at the end.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var d = 100;
var s = "sample";
debugMessage (d, s, "￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/system/print">print</a> function</td>
  </tr>
</table>




