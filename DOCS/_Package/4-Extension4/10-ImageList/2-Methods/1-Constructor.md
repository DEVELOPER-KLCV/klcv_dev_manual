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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var img = new ImageList( [ <b>URL or reader</b> [, <b>width</b>, <b>height</b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>URL or reader</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>width</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>height</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-4</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-7</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-11</td>
    <td></td>
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