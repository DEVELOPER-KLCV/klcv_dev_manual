---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.GetFontFamily Property
nav_order: 9
permalink: /package/standard/root/methods/getfontfamily
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the font name added by the <a href="/package/standard/root/methods/setfontfamily">SetFontFamily</a> method.<br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var fontname = //.GetFontFamily( <b>kind</b>, <b>face</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Return the font name as a string. If undefined, an empty string is returned.</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>kind</b></td>
    <td>Setting value of FontKind property to which font is assigned<br>Specify $ FONT2 to $ FONT7.</td>
  </tr>
  <tr>
    <td>integer <b>face</b></td>
    <td>Font type to acquire<br>Specify $ STD (for proportional display) or $ FIXED (for fixed pitch display)</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>PKG-59</td>
    <td>Invalid FontKind argument</td>
  </tr>
  <tr>
    <td>PKG-59</td>
    <td>Invalid FontName argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    for (var i = $FONT2; i <= $FONT7; i++) {
        print(i, //.GetFontFamily(i, $STD), "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/setfontfamily">SetFontFamily</a> method</td>
  </tr>
</table>



