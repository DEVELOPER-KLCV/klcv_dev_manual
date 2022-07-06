---
layout: default

grand_parent: HtmlView Class
parent: Methods
has_children: false
title: HtmlView.ScrollBy Method
nav_order: 8
permalink: /package/extension5/htmlview/methods/scrollby
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Scroll the displayed page relative to the current position.<br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">HtmlView1.ScrollBy(<b><i>x</i></b>, <b><i>y</i></b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b><i>x</i></b></td>
    <td>Specifies the number of pixels to scroll horizontally. <br>Positive values are to the right and negative values are to the left.</td>
  </tr>
  <tr>
    <td><b><i>y</i></b></td>
    <td>Specifies the number of pixels to scroll vertically. <br>Positive values are downwards, negative values are upwards.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-27</td>
    <td>Initialization has not been completed</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    ^.HtmlView1.ScrollBy(0, 100);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>