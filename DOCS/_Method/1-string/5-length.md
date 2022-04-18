---
layout: default

parent: String Manipulation

title: length
nav_order: 5
permalink: /method/str/length
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Find the length of the string.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = length( <b>character string</b>, <b>length</b> [, <b>processing unit</b> ] </td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">The length of the specified string</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>string</b></td>
    <td>String to check the length</td>
  </tr>
  <tr>
    <td>Integer <b>processing unit</b></td>
    <td>0:  Treat as one character without distinguishing between half-width and full-width<br>1:   Half-width characters are treated as one character, and full-width characters are treated as two characters.  If omitted, half-width and full-width characters will not be distinguished.<br> *<small>AI does not distinguish between half-width and full-width characters regardless of the argument</small>*</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var s = "ｱｸｼｽｿﾌﾄ株式会社";
print(length(s), length(s, 1), "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

