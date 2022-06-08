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
    <td colspan="2">Sets the image list used to display the window title icon<br><small><span style="color:red">Added since Ver.4.1.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
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
    <td colspan="2"><a href="/package/extension4/imagelist/">ImageList</a> object that holds the image list you want to display<br>Set the <a href="/package/extension4/imagelist/properties/maskuse">MaskUse</a> property to $ TRUE for the specified ImageList object. If $ FALSE, the background of the image may not be transparent and the expected drawing may not be performed.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-5</td>
    <td>ImageList reference is abnormal</td>
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



