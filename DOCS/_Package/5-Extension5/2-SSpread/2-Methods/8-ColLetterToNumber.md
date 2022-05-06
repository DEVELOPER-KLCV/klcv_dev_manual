---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ColLetterToNumber Method
nav_order: 8
permalink: /package/extension5/sspread/methods/ColLetterToNumber
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Converts an alphabetic string in a column header to the corresponding column number.<br><br>For example, "A" is converted to 1, "B" is converted to 2, and "AA" is converted to 27.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ColLetterToNumber(<b>letter</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Column index</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>letter</b></td>
    <td>Alphabet string in column header</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/methods/colnumbertoletter">ColNumberToLetter</a> method</td>
  </tr>
</table>
