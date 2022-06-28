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
    <td colspan="2">Load the image file.<br><br> JPEG or PNG is effective as the image file format.<br><small><span style="color:red">In addition to the above, GIF and BMP are also effective for AI</span></small>.<br><br> The image file is automatically divided by the size specified in the <a href="/package/extension4/imagelist/properties/iconwidth">IconWidth</a> and <a href="/package/extension4/imagelist/properties/iconheight">IconHeight</a> properties, and each can be obtained as an individual image with the <a href="/package/extension4/imagelist/methods/getimage">GetImage</a> method. Areas that do not meet the values of the IconWidth and IconHeight properties are filled in black. <br><br>If the LoadImage and <a href="/package/extension4/imagelist/methods/loadicon">LoadIcon</a> methods are called repeatedly, they will be added after the loaded image list. It will not be overwritten.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var num = ImageList1.LoadImage( <b><i>URL or Reader</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b><i>URL or Reader</i></b></td>
    <td>Specify the URL of the image file or the <a href="/base/readerwriter#reader-object">ReaderObject</a>.</td>
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