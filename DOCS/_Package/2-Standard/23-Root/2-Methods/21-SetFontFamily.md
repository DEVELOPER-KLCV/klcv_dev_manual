---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetFontFamily Property
nav_order: 21
permalink: /package/standard/root/methods/setfontfamily
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetFontFamily( <b>kind</b>, <b>p_font</b> [, <b>c_font</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b>kind</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>p_font</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>c_font</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>PKG-59</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-59</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetFontFamily($FONT2, "Arial");
 
Label b {
    :
    FontKind = $FONT2;
    Value = "Arial Font";
    :
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/getfontfamily">GetFontFamily</a> method</td>
  </tr>
</table>



