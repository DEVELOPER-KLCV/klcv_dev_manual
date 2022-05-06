---
layout: default

parent: 1. String Manipulation

title: trim
nav_order: 14
permalink: /method/str/trim
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Remove all leading and trailing whitespace in the <b>string</b>, and if there are consecutive whitespace in the middle of the <b>string</b>, make it one.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = trim( <b>string</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">String with whitespace removed</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>string</b></td>
    <td>Original character string</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var s = "  あいうえお     かきくけこ  ";
print("[" + trim(s) + "]\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

