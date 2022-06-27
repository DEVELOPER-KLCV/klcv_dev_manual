---
layout: default

grand_parent: ImageButton Class
parent: Methods
has_children: false
title: ImageButton.SetDisabledImage Method
nav_order: 6
permalink: /package/extension4/imagebutton/methods/setdisabledimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the image to be displayed on the button in the inactive state.<br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ImageButton1.SetDisabledImage( <b><i>img</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>Object <b><i>img</i></b></td>
    <td>Set the <a href="/package/extension4/image">Image</a> object, <a href="/package/extension4/imagelist">ImageList</a> object, or URL. <br> If you specify an ImageList object, the first image is used. <br> When set by URL, JPEG or PNG is effective as the image format.</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>Invalid URL argument</td>
  </tr>
  <tr>
    <td>EXT-7</td>
    <td>Invalid reference</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    ImageButton1.SetDisabledImage(ImageList1.GetImage(0));
    ImageButton2.SetDisabledImage("img/sample.png");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/imagebutton/methods/resetdisabledimage">ResetDisabledImage</a> method<br><a href="/package/extension4/image">Image</a>, <a href="/package/extension4/imagelist">ImageList</a> class</td>
  </tr>
</table>