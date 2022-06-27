---
layout: default

grand_parent: Image Class
parent: Methods
has_children: false
title: Image.ModifyBrightness Method
nav_order: 2
permalink: /package/extension4/image/methods/modifybrightness
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Change the image brightness. <br>However, it is invalid for the Image object obtained by the GetImage method of the ImageList class.<br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td> 
  </tr> 
  <tr>
    <td>Call format</td>
    <td colspan="2">img. ModifyBrightness ( <b><i>brightness</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>brightness</i></b></td>
    <td>Specify the amount of change in brightness in the range of -255 (dark) to 255 (bright).</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>Image: ModifyBrightness argument is invalid</td>
  </tr>
  <tr>
    <td>EXT-26</td>
    <td>Cannot be executed because the image does not exist</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Image img;
    img.LoadImage("biz.jpg");
    img.ModifyBrightness(-100);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>