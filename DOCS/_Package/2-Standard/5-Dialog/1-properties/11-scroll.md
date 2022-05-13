---
layout: default

grand_parent: Dialog Class
parent: Properties
has_children: false
title: Scroll property
nav_order: 11
permalink: /package/standard/dialog/properties/scroll
---
# {{ page.title }}

Controls the display of the scroll bar.

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
    <td class="tg-0pky">$ AUTO</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">Automatic display<br>The scroll bar is automatically displayed or hidden according to the size of the displayed content.</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ NONE</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">none<br>Not always displayed regardless of the size of the displayed content.<br>It is not possible to scroll to the contents beyond the display range.</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ STATIC</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">Fixed display<br>Always display regardless of the size of the displayed content.</td>
  </tr>
</tbody>
</table>

***Restrictions on Mobile version***<br>
The specification of $ STATIC is ignored<br>
<small> No more restriction since Mobile Ver.3.0.0