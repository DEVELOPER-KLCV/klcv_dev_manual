---
layout: default

grand_parent: ImageList Class
parent: Methiods
has_children: false
title: ImageList.GetImage Method
nav_order: 2
permalink: /package/extension4/imagelist/methods/getimage
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the image with the specified index number.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var img = ImageList1.GetImage( <b><i>no</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"><a href="/package/extension4/image">Image</a> object <br> The Image object obtained by this method cannot be rotated by the <br><a href="/package/extension4/image/methods/rotate">Rotate</a> method.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>no</i></b></td>
    <td>Image list index number<br> Specify an integer starting from 0.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
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
    <td colspan="2"><a href="/package/extension4/imagelist/methods/loadimage">LoadImage</a>, <a href="/package/extension4/imagelist/methods/loadicon">LoadIcon</a> methods<br><a href="/package/extension4/image">Image</a> class</td>
  </tr>
</table>