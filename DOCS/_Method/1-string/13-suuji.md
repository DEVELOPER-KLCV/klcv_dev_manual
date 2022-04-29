---
layout: default

parent: 1. String Manipulation
title: suuji
nav_order: 13
permalink: /method/str/suuji
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Converts a <b>number</b> to a string of Chinese numerals. Numbers after the decimal point are rounded off.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = suuji( <b>number value</b> [, <b>representation</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Character string converted to Chinese numerals</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Number <b>number</b></td>
    <td>Numerical values ​​to convert to Chinese numerals</td>
  </tr>
  <tr>
    <td>Integer <b>display format</b></td>
    <td>If the number is 321<br>1: 321<br>2: San Hyaku 2 Pickup Ichi<br>3: 32<br>If omitted, the display format will be 1.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var s = suuji(12345);
print(s, "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

