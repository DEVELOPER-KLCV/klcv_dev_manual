---
layout: default

grand_parent: ImageButton Class
parent: Methods
has_children: false
title: ImageButton.SetPushedImage Method
nav_order: 9
permalink: /package/extension4/imagebutton/methods/setpushedimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the image to be displayed on the pressed button.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ImageButton1.SetPushedImage( <b><i>img</i></b> )</td>
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
    ImageButton1.SetPushedImage(ImageList1.GetImage(0));
    ImageButton2.SetPushedImage("img/sample.png");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/imagebutton/methods/resetpushedimage">ResetPushedImage</a> method<br><a href="/package/extension4/image">Image</a>, <a href="/package/extension4/imagelist">ImageList</a> class</td>
  </tr>
</table>