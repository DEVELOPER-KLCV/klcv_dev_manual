---
layout: default

grand_parent: ImageList Class
parent: Methiods
has_children: false
title: ImageList.LoadImage Method
nav_order: 4
permalink: /package/extension4/imagelist/methods/loadimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var num = ImageList1.LoadImage( <b>URL or Reader</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>URL or Reader</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-7</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    ImageList ImageList1 {
        IconWidth = 32;
        IconHeight = 32;
        LoadImage("http://localhost/picture.jpg");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/imagelist/properties/iconwidth">IconWidth</a>, <a href="/package/extension4/imagelist/properties/iconheight">IconHeight</a> properties<br><a href="/package/extension4/imagelist/methods/getimage">GetImage</a>, <a href="/package/extension4/imagelist/methods/loadicon">LoadIcon</a>, <a href="/package/extension4/imagelist/methods/removeimage">RemoveImage</a> methods</td>
  </tr>
</table>