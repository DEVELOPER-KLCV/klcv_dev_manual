---
layout: default

grand_parent: Form Class
parent: Methods
has_children: false
title: Form.FindSVGElement Method
nav_order: 1
permalink: /package/standard/form/methods/FindSVGElement
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
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
    <td></td>
  </tr>
  <tr>
    <td>integer <b>yPos</b></td>
    <td></td>
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
    <td colspan="2"><a href="/package/standard/form/properties/BgPattern">BgPattern</a> property<br><a href="/package/standard/form/methods/GetSVGElementPosition">GetSVGElementPosition</a> method<br><a href="">XmlElement</a> class<br></td>
  </tr>
</table>



