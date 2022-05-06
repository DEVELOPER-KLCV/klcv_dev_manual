---
layout: default

parent: 1. String Manipulation

title: str
nav_order: 11
permalink: /method/str/str
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Converts a number, date, or string to a string.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = str (<b>value</b> [, <b>format string</b>])</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Converted string</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>value</b></td>
    <td>Value to convert</td>
  </tr>
  <tr>
    <td>String <b>format string</b></td>
    <td>Refer to <a>Format</b> property (optional)</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var n = new Number(1234.56);
var f = new Fixed(4567.89);
var d = sysdate();
var s = "string";
print(str(n), str(f), str(d), str(s), "\n");
print(str(n, "999,990.99"), "\n");
print(str(d, "WSWYY.MM.DD"), "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/str/val">val</a> method<br><a>Format</a> property</td>
  </tr>
</table>

