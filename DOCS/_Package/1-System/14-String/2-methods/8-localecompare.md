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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = str.LocaleCompare( <b>comp</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>comp</b></td>
    <td></td>
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