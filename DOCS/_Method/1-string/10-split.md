---
layout: default

parent: String Manipulation

title: split
nav_order: 10
permalink: /method/str/split
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Separates the <b>string</b> with a <b>delimiter string</b> and gets its elements.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = split( <b>string</b>, <b>delimiter string</b>, <b>element position</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Element corresponding to the specified element position<br>If there is no corresponding element at the specified element position, an empty string is returned.</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>string</b></td>
    <td>Original character string</td>
  </tr>
  <tr>
    <td>String <b>delimiter string</b></td>
    <td>String to use as a delimiter</td>
  </tr>
  <tr>
    <td>Integer <b>element position</b></td>
    <td>Position of the element to be taken out<br>Specify by the number where the leftmost element is 0.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var s = "1999/08/10";
print(split(s, "/", 0), "\n");  /* 1999 が切り出されます */
print(split(s, "/", 1), "\n");  /* 08 が切り出されます */
print(split(s, "/", 2), "\n");  /* 10 が切り出されます */</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

