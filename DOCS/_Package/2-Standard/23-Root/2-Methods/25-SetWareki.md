---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetWareki Property
nav_order: 25
permalink: /package/standard/root/methods/setwareki
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Specify the year and period of the Japanese calendar.<br><br>The year specified using this method will be applied until the Biz / Browser is restarted or the Login method is called. Please note that the year cannot be deleted or changed during execution.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetWareki( <b>sym</b>, <b>sym2</b>, <b>from</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>sym</b></td>
    <td>Year string</td>
  </tr>
  <tr>
    <td>String <b>sym2</b></td>
    <td>Year abbreviation</td>
  </tr>
  <tr>
    <td>String <b>from</b></td>
    <td>Specify the start date of the year specified by sym in Date type. The specified date is included in the year specified by sym.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetWareki("年号", "N", "2080/1/1");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



