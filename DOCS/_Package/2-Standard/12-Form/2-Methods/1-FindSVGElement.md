---
layout: default

grand_parent: Form Class
parent: Methods
has_children: false
title: Form.FindSVGElement Method
nav_order: 1
permalink: /package/standard/form/methods/findsvgelement
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the SVG element displayed at the specified coordinates.<br><br>The element to get is an <a href="/package/xmlpackage/xmlelement">XmlElement</a>  object that will be part of the SVG specified in the background in the <a href="/package/standard/form/properties/bgpattern">BgPattern</a> property.<br>If the BgPattern property is not specified, it's impossible to get the element from an SVG that is different from the BgPattern property.<br><br>Since the display coordinates of SVG are determined in the actual display process, correct results can't be obtained even if the FindSVGElement method is called immediately after setting SVG in the BgPattern property or when SVG is never displayed on the screen such as a hidden Form.<br><br>The SVG elements to be searched are limited to the elements to be drawn such as <rect> and <circle> that have a fill color without transparency specification. For example, <rect> requires the fill attribute to be specified. If only the stroke attribute is specified and only the frame is displayed, it will not be searched.<br><br> For <b>xPos</b> and <b>yPos</b> , specify the coordinates withthe upper left of the Form(0,0).<br> <small><span style="color:blue">Not supported in Mobile, AI</span></small>
 
  <tr>
    <td>Call format</td>
    <td colspan="2">var elm = Form1.FindSVGElement( <b>xPos</b>, <b>yPos</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>xPos</b></td>
    <td>X coordinate</td>
  </tr>
  <tr>
    <td>integer <b>yPos</b></td>
    <td>Y coordinate</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
Function OnClicked(e) {
    var elm = FindSVGElement(e.xPos, e.yPos);
    if (elm == null) return;
    print(elm.TagName, "\n");
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/form/properties/bgpattern">BgPattern</a> property<br><a href="/package/standard/form/methods/getsvgelementposition">GetSVGElementPosition</a> method<br><a href="/package/xmlpackage/xmlelement">XmlElement</a> class<br></td>
  </tr>




