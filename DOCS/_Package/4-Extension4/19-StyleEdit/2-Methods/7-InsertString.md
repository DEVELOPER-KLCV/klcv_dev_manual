---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.InsertString Method
nav_order: 7
permalink: /package/extension4/styleedit/methods/insertstring
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Inserts the string at the specified position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">StyleEdit1.InsertString( <b><i>pos</i></b>, <b><i>str</i></b> [, <b><i>styleNo</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b><i>pos</i></b></td>
    <td>Specify the position of the inserted character. If the position points to the second byte of a multi-byte character, it is automatically corrected to the next position. If -1 is specified, it will be the current cullet position.</td>
  </tr>
  <tr>
    <td>String <b><i>str</i></b></td>
    <td>The string to insert.</td>
  </tr>
  <tr>
    <td>integer <b><i>styleNo</i></b></td>
    <td>Specify when setting the style at the same time as inserting the character string. The range that can be specified is from 0 to 30.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid arguments</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    StyleEdit1.InsertString(10, "Insert this string", 1);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2">None</td>
  </tr>
</table>