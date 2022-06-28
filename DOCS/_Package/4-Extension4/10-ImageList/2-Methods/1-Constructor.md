---
layout: default

grand_parent: ImageList Class
parent: Methiods
has_children: false
title: ImageList Constructor
nav_order: 1
permalink: /package/extension4/imagelist/methods/constructor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize the ImageList object. <br><br>JPEG or PNG is effective as the image file format. Biz / Browser V or later also supports formats such as BMP, GIF, TIFF, and EXIF.<br><small><span style="color:red">In addition to BMP and GIF formats, AI also supports transparent PNG formats.</span></small> <br><br> The image file is automatically divided into the sizes specified in <b><i>width</i></b> and <b><i>height</i></b>, and each can be obtained as an individual image with the <br><a href="/package/extension4/imagelist/methods/getimage">GetImage</a> method. Areas that do not meet the <b><i>width</i></b> and <b><i>height</i></b>  values are filled in black.<br><br><small><span style="color:red">Added since Ver.4.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var img = new ImageList( [ <b><i>URL or reader</i></b> [, <b><i>width</i></b>, <b><i>height</i></b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b><i>URL or Reader</i></b></td>
    <td>Image file URL or <a href="/base/readerwriter#reader-object">ReaderObject</a> <br> By default, it is an empty image list, and you need to call the <a href="/package/extension4/imagelist/methods/loadimage">LoadImage</a> and <a href="/package/extension4/imagelist/methods/loadicon">LoadIcon</a> methods to load the image.</td>
  </tr>
  <tr>
    <td>integer <b><i>width</i></b></td>
    <td>Image width <br> The range that can be specified is 16 to 1024, and the default is 16. The specified value is set in the <a href="/package/extension4/imagelist/properties/iconwidth">IconWidth</a> property.</td>
  </tr>
  <tr>
    <td>integer <b><i>height</i></b></td>
    <td>Image height <br> The range that can be specified is 16 to 1024, and the default is 16. The specified value is set in the <a href="/package/extension4/imagelist/properties/iconheight">IconHeight</a> property.</td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>EXT-1</td>
    <td>Invalid URL argument</td>
  </tr>
  <tr>
    <td>EXT-4</td>
    <td>The width of the image list exceeds 32767 dots</td>
  </tr>
  <tr>
    <td>EXT-7</td>
    <td>Invalid reference</td>
  </tr>
  <tr>
    <td>EXT-11</td>
    <td>Read method not found</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var img = new ImageList("sample.png", 32, 32);
    ImageLabel1.SetImage(img.GetImage(0));
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/imagelist/properties/iconwidth">IconWidth</a>, <a href="/package/extension4/imagelist/properties/iconheight">IconHeight</a> properties<br><a href="/package/extension4/imagelist/methods/getimage">GetImage</a>, <a href="/package/extension4/imagelist/methods/loadimage">LoadImage</a>, <a href="/package/extension4/imagelist/methods/loadicon">LoadIcon</a> methods</td>
  </tr>
</table>