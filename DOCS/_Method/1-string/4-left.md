---
layout: default

parent: String Manipulation

title: left
nav_order: 4
permalink: /method/str/left
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Extracts the specified <b>length</b> from the beginning (left end) of the <b>character string</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = left( <b>character string</b>, <b>length</b> [, <b>processing unit</b> ] </td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Extracted character string</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>string</b></td>
    <td>Original character string</td>
  </tr>
  <tr>
    <td>Integer <b>length</b></td>
    <td>Number of characters to extract</td>
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
    <td colspan="2"><a href="/img/Biz Browser V/Left.PNG" target="_blank"><br><img src="/img/Biz Browser V/Left.PNG" alt="Left method"></a></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><code><pre>var str = "I have a book. I have a pen.";
var s = left(str, 14);
print(s, "\n");</pre></code></td>
  </tr>
</table>

