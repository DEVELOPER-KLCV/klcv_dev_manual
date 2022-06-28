---
layout: default

grand_parent: ImageList Class
parent: Methiods
has_children: false
title: ImageList.LoadIcon Method
nav_order: 3
permalink: /package/extension4/imagelist/methods/loadicon
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Loads the icon image associated with the extension. <br><br>The icon image is enlarged or reduced according to the size specified by the <a href="/package/extension4/imagelist/properties/iconwidth">IconWidth</a> and <a href="/package/extension4/imagelist/properties/iconheight">IconHeight</a> properties. If you want to display the original icon size, set the IconWidth and IconHeight properties to appropriate values (for example, 32x32 for large icons). <br><br>If the <a href="/package/extension4/imagelist/methods/loadimage">LoadImage</a> and LoadIcon methods are called repeatedly, they will be added after the loaded image list. It will not be overwritten.<br><br><small><span style="color:blue">Not supported by AI. If called, it will be ignored.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var num = ImageList1.LoadIcon( <b><i>exp</i> [, <b><i>large</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td> 
    <td colspan="2">Index number of newly added image</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b><i>exp</i></b></td>
    <td>Specify the extension. You can also specify a drive other than the extension. <br>If there is no application associated with the extension, or if the drive does not exist, an alternate icon will be displayed.</td>
  </tr>
  <tr>
    <td>boolean <b><i>large</i></b></td>
    <td>Set $ TRUE to get the image from the large icon and $ FALSE to get the image from the small icon. <br>If omitted, it follows the setting of the <a href="/package/extension4/imagelist/properties/largeimage">LargeImage</a> property.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    ImageList1.LoadIcon("txt");
    ImageList1.LoadIcon("doc");
    ImageList1.LoadIcon("C:\\");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/imagelist/properties/largeimage">LargeImage</a> property<br><a href="/package/extension4/imagelist/methods/getimage">GetImage</a>, <a href="/package/extension4/imagelist/methods/loadimage">LoadImage</a>, <a href="/package/extension4/imagelist/methods/removeimage">RemoveImage</a> methods</td>
  </tr>
