---
layout: default

grand_parent: Dialog Class
parent: Events
has_children: false
title: Clicked Event
nav_order: 1
permalink: /package/standard/dialog/events/clicked
---
# {{ page.title }}

Occurs when the left mouse button is pressed.

 

The following child objects are attached to the Event object.<br>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-6t3r{font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Type</th>
    <th class="tg-xt05">Name</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">ShiftKey</td>
    <td class="tg-0lax">1 if the Shift key is pressed, 0 otherwise</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">CtrlKeyKey</td>
    <td class="tg-0lax">1 if the Ctrl key is pressed, 0 otherwise</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">AltKey</td>
    <td class="tg-0lax">1 if the Alt key is pressed, 0 otherwise</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">xPos</td>
    <td class="tg-0lax">X coordinate of mouse pointer</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">yPos</td>
    <td class="tg-0lax">Y coordinate of mouse pointer</td>
  </tr>
</tbody>
</table>

Example of use
```
Function OnClicked (e) {
    MessageBox (strf (" clicked on (% 1,% 2) ", e.xPos, e.yPos));
}
```
