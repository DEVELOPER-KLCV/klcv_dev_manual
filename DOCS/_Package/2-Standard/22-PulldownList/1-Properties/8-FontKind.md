---
layout: default

grand_parent: PulldownList Class
parent: Properties
has_children: false
title: FontKind Property
nav_order: 8
permalink: /package/standard/pulldownlist/properties/fontkind
---
# {{ page.title }}
<br>

Specify the font type.

The font type can be specified as $ STD, $ FONT1 to $ FONT7.

The font type can be specified as $ STD, $ FONT1 to $ FONT7.

$ STD is a Gothic font, $ FONT1 is a Mincho font, and $ FONT2 to $ FONT7 use the font specified by the <a href="/package/standard/root/methods/setfontfamily">Root.SetFontFamily</a> method. The display result is undefined if the font not assigned by the SetFontFamily method in $ FONT2 to $ FONT7 or the assigned font is not registered in the computer.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-cqgq">Constant</th>
    <th class="tg-cqgq">Value</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-lcf4">$STD</td>
    <td class="tg-lcf4">0</td>
    <td class="tg-j5n6">Gothic</td>
  </tr>
  <tr>
    <td class="tg-lcf4">$ FONT1</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Mincho</td>
  </tr>
  <tr>
    <td class="tg-lcf4">$FONT2</td>
    <td class="tg-lcf4">2</td>
    <td class="tg-j5n6" rowspan="6">Font set by <a href="/package/standard/root/methods/setfontfamily">Root.SetFontFamily</a> method</td>
  </tr>
  <tr>
    <td class="tg-lcf4">$FONT3</td>
    <td class="tg-lcf4">3</td>
  </tr>
  <tr>
    <td class="tg-lcf4">$ FONT4</td>
    <td class="tg-lcf4">4</td>
  </tr>
  <tr>
    <td class="tg-lcf4">$FONT5</td>
    <td class="tg-lcf4">5</td>
  </tr>
  <tr>
    <td class="tg-lcf4">$FONT6</td>
    <td class="tg-lcf4">6</td>
  </tr>
  <tr>
    <td class="tg-lcf4">$FONT7</td>
    <td class="tg-lcf4">7</td>
  </tr>
</tbody>
</table>

<br><small><span style="color:green">Since Ver.4.1.0, the constant corresponding to Mincho has been changed from $ BOLD to $ FONT1. $ BOLD constant compatibility is valid.</span></small>
<br><small><span style="color:red">Since Ver.4.1.0, constants of $ FONT2-7 have been added.</span></small>
<br><small><span style="color:blue">Not supported in Mobile</span></small>
<br><small><span style="color:blue">AI does not support $ FONT2-7 constants</span></small>
