---
layout: default

parent: String Manipulation

title: mid
nav_order: 7
permalink: /method/str/mid
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Extracts a character string of the specified <b>length</b> from the specified <b>position</b> of the <b>character string</b>. The position is counted with 0 at the beginning of the string.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var i = mid ( <b>string</b>, <b>target location</b>, <b>length</b> [, <b>processing unit</b> ]) </td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Extracted character string</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>String <b>string</b></td>
    <td>Original character string</td>
  </tr>
  <tr>
    <td>Integer <b>position</b></td>
    <td>Position to start ejecting</td>
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
    <td colspan="2"><code><pre>var str = "I have a book. I have a pen.";
var s = mid(str, 9, 4);
print(s, "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/method/str/left">left</a>, <a href="/method/str/right">right</a> method</td>
  </tr>
</table>

