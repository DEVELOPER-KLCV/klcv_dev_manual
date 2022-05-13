---
layout: default

grand_parent: UString Class
parent: Methods
has_children: false
title: UString.FromCharCode Method
nav_order: 20
permalink: /package/system/ustring/methods/fromcharcode
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Create a character string from the character code.<br>This method is a static method. It can be called without creating an object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var str = String.FromCharCode( <b>code_1</b> [, <b>code_2</b> [, … [, <b>code_n</b> ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Created string</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>code_n</b></td>
    <td>Shift_JIS character code<br>Only the lower 16 bits (2 bytes) are valid.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = UString.FromCharCode(0x0041, 0x0042, 0x0043);
print(str, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>