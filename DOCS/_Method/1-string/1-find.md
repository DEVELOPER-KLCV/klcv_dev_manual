---
layout: default

parent: String Manipulation

title: find
nav_order: 1
permalink: /method/str/find
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"><b>The target character string</b> is searched from the <b>start position of the character string</b>, and the start position of the matching part is obtained. The position is 0 at the beginning of the <b>string</b>.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var i = find ( <b>string</b>, <b>target string</b>, <b>start position</b> [, <b>processing unit</b> ]) </td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">The beginning position of the matched part </td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>String <b>string</b></td>
    <td>Character string to search</td>
  </tr>
  <tr>
    <td>String <b>target string</b></td>
    <td> Character string to be searched</td>
  </tr>
  <tr>
    <td>Integer <b>start position</b></td>
    <td>The position to start the search in the target character string</td>
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
var i = -1;
while (true) {
    i = find(str, "have", i + 1);
    if (i < 0) {
        break;
    }
    print(i, "\n");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





