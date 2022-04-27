---
layout: default

grand_parent: Image Class
parent: Methods
has_children: false
title: Image.ModifyBrightness Method
nav_order: 2
permalink: /package/extension4/image/methods/modifybrightness
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">img. ModifyBrightness ( <b>brightness</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>brightness</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-26</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Image img;
    img.LoadImage("biz.jpg");
    img.ModifyBrightness(-100);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>