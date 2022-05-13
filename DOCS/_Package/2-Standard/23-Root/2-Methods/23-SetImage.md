---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetImage Property
nav_order: 23
permalink: /package/standard/root/methods/setimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetImage( <b>img</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>ImageList <b>img</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-5</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    ImageList img {
    MaskUse = $TRUE;
    MaskColB = 255;
    MaskColR = 255;
    LoadImage("icon.png");
}
//.SetImage(img);
//.Icon = 1;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/properties/icon">Icon</a> property<br><a href="/package/standard/root/methods/resetimage">ResetImage</a> method<br><a href="/package/extension4/imagelist/">ImageList</a> class</td>
  </tr>
</table>



