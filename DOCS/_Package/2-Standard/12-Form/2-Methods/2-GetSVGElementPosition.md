---
layout: default

grand_parent: Form Class
parent: Methods
has_children: false
title: Form.GetSVGElementPosition Method
nav_order: 2
permalink: /package/standard/form/methods/getsvgelementposition
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the coordinates where the specified SVG element is displayed.<br><br>The element you specify is an <a href="/package/xmlpackage/xmlelement">XmlElement</a> object that will be part of the SVG you specified for the background in the <a href="/package/standard/form/properties/bgpattern">BgPattern</a> property.<br> If you don't specify the BgPattern property, you can't specify an SVG element that is different from the BgPattern property.<br><br>Since the display coordinates of SVG are determined in the actual display process, correct results can't be obtained even if the GetSVGElementPosition method is called immediately after setting SVG in the BgPattern property or when SVG such as a hidden Form has never been displayed on the screen.<br><br>The SVG elements to be processed are limited to the elements to be drawn such as <rect> and <circle> that have a fill color without transparency specification (if <rect>, fill attribute and stroke attribute are not included).<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>
  <tr>
    <td>Call format</td>
    <td colspan="2">ver pos = Form1.GetSVGElementPosition( <b>elm</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-f7v4{background-color:#c0c0c0;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-fymr{border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-f7v4">Type</th>
    <th class="tg-f7v4">Name</th>
    <th class="tg-f7v4">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-fymr">Left</td>
    <td class="tg-0pky">Leftmost coordinates</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-fymr">Top</td>
    <td class="tg-0pky">Top coordinates</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-fymr">Width</td>
    <td class="tg-0pky">Width</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-fymr">Height</td>
    <td class="tg-0pky">Height</td>
  </tr>
</tbody>
</table><br>If the coordinates cannot be obtained, null is returned.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlElement <b>elm</b></td>
    <td><a href="/package/xmlpackage/xmlelement">XmlElement</a> object to get coordinates</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/form/properties/bgpattern">BgPattern</a> property<br><a href="/package/standard/form/methods/findsvgelement">FindSVGElement</a> method<br><a href="/package/xmlpackage/xmlelement">XmlElement</a> class<br></td>
  </tr>


