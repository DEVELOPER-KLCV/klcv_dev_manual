---
layout: default

grand_parent: Dialog Class
parent: Properties
has_children: false
title: Dialog.SetImage Method
nav_order: 4
permalink: /package/standard/dialog/methods/setimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">Dialog1.SetImage( <b>image</b> )</td>
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
    <td colspan="2"><code><pre>
ImageList img {
    MaskUse = $TRUE;
    MaskColB = 255;
    MaskColR = 255;
    LoadImage("icon.png");
}
Dialog1.SetImage(img);
Dialog1.Icon = 1;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/dialog/properties/icon">Icon</a> property<br><a href="/package/standard/dialog/methods/resetimage">ResetImage</a> method<br><a href="/package/extension4/imagelist">ImageList</a> class</td>
  </tr>
</table>