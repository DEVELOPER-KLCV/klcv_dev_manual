---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ColNumberToLetter Method
nav_order: 9
permalink: /package/extension5/sspread/methods/colnumbertoletter
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the alphabetic string in the column header that corresponds to the column number.<br><br>For example, 1 can get "A", 2 can get "B", and 27 can get "AA".</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ColNumberToLetter(<b>num</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Alphabet string in column header</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>num</b></td>
    <td>Column index</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    print(ColLetterToNumber("A"), "\n");
    print(ColLetterToNumber("B"), "\n");
    print(ColLetterToNumber("Z"), "\n");
    print(ColLetterToNumber("AA"), "\n");
    print(ColLetterToNumber("AB"), "\n");
    print(ColNumberToLetter(1), "\n");
    print(ColNumberToLetter(2), "\n");
    print(ColNumberToLetter(26), "\n");
    print(ColNumberToLetter(27), "\n");
    print(ColNumberToLetter(28), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/collettertonumber">ColLetterToNumber</a> method</td>
  </tr>
</table>
