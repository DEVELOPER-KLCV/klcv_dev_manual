---
layout: default

grand_parent: Dialog Class
parent: Methods
has_children: false
title: Dialog.SetImage Method
nav_order: 4
permalink: /package/standard/dialog/methods/setimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the image list used to display the icon of the dialog title<br><small>Added since Ver.4.1.3<br>Not supported in Mobile, AI</small></td>
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
    <td><a href="/package/extension4/imagelist">ImageList</a> object that holds the image list you want to display<br>Set the <a href="/package/extension4/imagelist/properties/maskuse">MaskUse</a> property to $ TRUE for the specified ImageList object. In the case of $ FALSE, the background part of the image may not be transparent and the expected drawing may not be performed.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-5</td>
    <td>	
ImageList reference is abnormal</td>
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