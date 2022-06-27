---
layout: default

grand_parent: Image Class
parent: Methods
has_children: false
title: Image.Save Method
nav_order: 5
permalink: /package/extension4/image/methods/save
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Saves the image in the Writer object in the specified format. <br>However, it is invalid for the Image object obtained by the <a href="/package/extension4/imagelist/methods/getimage">GetImage</a> method of the <a href="/package/extension4/imagelist">ImageList</a> class.<br><small><span style="color:red">Added since Ver.5.0.4</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">img. Save ( <b><i>writer</i></b>, <b><i>format</i></b>,[, <b><i>option1</i></b>[, <b><i>option2</i></b>]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>Object <b><i>writer</i></b></td>
    <td><a href="/base/readerwriter#writer-object">WriterObject</a> to save to</td>
  </tr>
  <tr>
    <td>Integer <b><i>format</i></b></td>
    <td>Specify the image format from the following values.
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
    <td class="tg-0pky">Image.FORMAT_BMP</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">24- bit bitmap</td>
  </tr>
  <tr>
    <td class="tg-0pky">Image.FORMAT_JPEG</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">JPEG</td>
  </tr>
  <tr>
    <td class="tg-0pky">Image.FORMAT_PNG</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">PNG</td>
  </tr>
</tbody>
</table>
    </td>
  </tr>
  <tr>
    <td>Any <b><i>option1</i></b></td>
    <td>When FORMAT_JPEG is specified, image quality is 100 (high) to 1 (low), default is 100.</td>
  </tr>
  <tr>
    <td>Any <b><i>option2</i></b></td>
    <td>When FORMAT_JPEG is specified, true = progressive JPEG, default false</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>Image: Save argument is invalid</td>
  </tr>
  <tr>
    <td>EXT-26</td>
    <td>Cannot be executed because the image does not exist</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var fs = new FileSystem;
    var fp = fs.Open("sample.jpg", FileSystem.OPEN_WRITE);
    img.Save(fp, Image.FORMAT_JPEG, 80, true);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>