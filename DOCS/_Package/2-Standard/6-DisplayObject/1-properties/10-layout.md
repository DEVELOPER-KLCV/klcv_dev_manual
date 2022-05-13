---
layout: default

grand_parent: DisplayObject Class
parent: Properties
has_children: false
title: DisplayObject.Layout property
nav_order: 10
permalink: /package/standard/displayobject/properties/layout
---
# {{ page.title }}

Specifies how to arrange each element when the object is created as an array.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-2m49{background-color:#D9D9D9;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-2m49">Value</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ VERTICAL</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Arrange the objects vertically.<br>The<a href="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/displayobjp2.htm">Y</a> property of each element of the array has no effect.</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ HORIZONTAL</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Arrange the objects horizontally.<br>The<a href="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/displayobjp1.htm">X</a> property of each element of the array has no effect.</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ BLANK</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">Do not line up. Each element of the array must be explicitly coordinated by a script.</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ OPTIMAL</td>
    <td class="tg-baqh">Four</td>
    <td class="tg-0lax">$ HORIZONTAL and adjust the position according to the string length of the label so that it is in the optimum arrangement.<br><small>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-change500.gif" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-change450.gif" width="86" height="12">. Only CheckItem class and OptionItem class can be used.<br>Not supported in <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/aiver-non.gif" width="18" height="12"></small></td>
  </tr>
</tbody>
</table>

Some classes automatically control the display position, and the Layout property setting may be invalid.
