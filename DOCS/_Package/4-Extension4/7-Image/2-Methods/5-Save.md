---
layout: default

grand_parent: Image Class
parent: Methods
has_children: false
title: Image.Save Method
nav_order: 5
permalink: /package/extension4/image/methods/save
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">img. Save ( <b>writer</b>, <b>format</b>,[, <b>option1</b>[, <b>option2</b>]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>Object <b>writer</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Integer <b>format</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Any <b>option1</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Any <b>option2</b></td>
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
    var fs = new FileSystem;
    var fp = fs.Open("sample.jpg", FileSystem.OPEN_WRITE);
    img.Save(fp, Image.FORMAT_JPEG, 80, true);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>