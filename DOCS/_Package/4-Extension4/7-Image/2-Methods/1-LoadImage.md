---
layout: default

grand_parent: Image Class
parent: Methods
has_children: false
title: Image.LoadImage Method
nav_order: 1
permalink: /package/extension4/image/methods/loadimage
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Load the image file.<br>JPEG or PNG is effective as the image file format.<br>Biz / Browser V or later also supports formats such as BMP, GIF, TIFF, and EXIF.<br><small><span style="color:red">In addition to BMP and GIF formats, AI also supports transparent PNG formats.<br></span></small>If called repeatedly, the previous image will be overwritten and the last image will be valid.</td> 
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">img.LoadImage( <b><i>URL or reader</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td> 
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b><i>URL or reader</i></b></td>
    <td>Image file URL or <a href="/base/readerwriter#reader-object">ReaderObject</a></td>
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
    img.LoadImage("http://localhost/picture.jpg");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/image/methods/removeimage">RemoveImage</a> method</td>
  </tr>
</table> 