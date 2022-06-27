---
layout: default

grand_parent: Image Class
parent: Methods
has_children: false
title: Image.Rotate Method
nav_order: 4
permalink: /package/extension4/image/methods/rotate
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Rotate the image.<br><br> However, it is invalid for the Image object obtained by the  <a href="/package/extension4/imagelist/methods/getimage">GetImage</a> method of the <a href="/package/extension4/imagelist">ImageList</a> class.<br><br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">img.Rotate( <b><i>direction</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>directionr</i></b></td>
    <td>Specify the amount to rotate from the following values.
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-34fe{background-color:#c0c0c0;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-llyw{background-color:#c0c0c0;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-llyw">Constant</th>
    <th class="tg-34fe">Value</th>
    <th class="tg-llyw">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Image.deg90</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">Rotate 90 degrees clockwise</td>
  </tr>
  <tr>
    <td class="tg-0pky">Image.deg180</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Rotate 180 degrees</td>
  </tr>
  <tr>
    <td class="tg-0pky">Image.deg270</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">Rotate 270 degrees clockwise</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-1</td>
    <td>Image: Rotate argument is invalid</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Image img;
    img.LoadImage("biz.jpg");
    img.Rotate(Image.deg180);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>