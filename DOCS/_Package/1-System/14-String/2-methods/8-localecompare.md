---
layout: default

grand_parent: String Class
parent: Properties
has_children: false
title: String.LocaleCompare Method
nav_order: 8
permalink: /package/system/string/methods/localecompare
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Compare strings based on locale.<br>The current implementation is byte-by-byte comparison regardless of locale.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = str.LocaleCompare( <b>comp</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns1if greater than <b>comp</b> <br>Returns-1if less than<b>comp</b> <br>Returns 0 if equal to <b>comp</b></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>comp</b></td>
    <td>String to compare</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
var str = new String("abcdefg");
print(str.LocaleCompare("abcdefg"), "\n"); /* return 0 */
print(str.LocaleCompare("ABC"), "\n");     /* return 1 */
print(str.LocaleCompare("bcd"), "\n");     /* return -1 */
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/string/methods/equalsignorecase">EqualsIgnoreCase</a> method</td>
  </tr>
</table>