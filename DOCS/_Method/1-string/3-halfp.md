---
layout: default

parent: String Manipulation

title: halfp
nav_order: 3
permalink: /method/str/halfp
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Converts full-width characters in a character string to half-width characters.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = halfp( <b>character string</b> [, <b>flag</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Character string converted from full-width characters to half-width characters</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>string</b></td>
    <td>Original character string</td>
  </tr>
  <tr>
    <td>Boolean <b>flag</b></td>
    <td>Specify the processing of voiced sound mark and semi-voiced sound mark.<br>In the case of $ TRUE, the voiced and semi-voiced sound marks are processed.<br>If $ FALSE or omitted, voiced and semi-voiced sound marks are not processed.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print(halfp("ＡＢＣａｂｃ１２３＋－"), "\n");
print(halfp("アイウ、ガギグ。「パピプ」", $TRUE), "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/str/fullp">fullp</a> method</td>
  </tr>
</table>

