---
layout: default

parent: String Manipulation

title: replace
nav_order: 8
permalink: /method/str/replace
---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Deletes the specified <b>length</b> from the specified <b>position</b> in the <b>string</b> and inserts the <b>replacement string</b> at that <b>position</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = replace( <b>string</b>, <b>position</b>, <b>length</b>, <b>replacement string</b> [, <b>processing unit</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Replaced string</td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td>String <b>string</b></td>
    <td>Original character string</td>
  </tr>
  <tr>
    <td>Integer <b>position</b></td>
    <td>Position to operate in the character string</td>
  </tr>
  <tr>
    <td>Integer <b>length</b></td>
    <td>Length to delete</td>
  </tr>
  <tr>
    <td>String <b>replacement string</b></td>
    <td>String to replace</td>
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
    <td colspan="2"><code><pre>var s = "I have a book. I have a pen.";
s = replace(s, 9, 4, "pencil");
s = replace(s, 0, 1, "You");
print(s, "\n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>

