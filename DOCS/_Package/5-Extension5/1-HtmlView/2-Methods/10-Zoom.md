---
layout: default

grand_parent: HtmlView Class
parent: Methods
has_children: false
title: HtmlView.Zoom Method
nav_order: 10
permalink: /package/extension5/htmlview/methods/zoom
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Scales the display. <br>This feature is only available when Internet Explorer 7 or later is installed.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">HtmlView1.Zoom( [ <b><i>ratio</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b><i>ratio</i></b></td>
    <td>Specify the enlargement / reduction ratio as a numerical value from 0.1 to 1 to 10. <br>If omitted, it is regarded as 1.0 (1x).</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-27</td>
    <td>Initialization has not been completed</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    ^.HtmlView1.Zoom(2);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>