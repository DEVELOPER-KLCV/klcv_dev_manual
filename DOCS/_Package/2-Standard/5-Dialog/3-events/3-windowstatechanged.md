---
layout: default

grand_parent: Dialog Class
parent: Events
has_children: false
title: Dialog.WindowStateChanged Event
nav_order: 3
permalink: /package/standard/dialog/events/windowstatechanged
---
# {{ page.title }}

Occurs when a state change occurs, such as maximizing or minimizing a dialog.

The following child objects are attached to the Event object.

<table>
    <tr>
        <td>Type</td>
        <td>Name</td>
        <td>Description</td>
    </tr>
    <tr>
        <td>Number</td>
        <td><b>state</b></td>
        <td>The following values ​​are set.
        <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
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
    <td class="tg-0lax">$ MINIMIZE</td>
    <td class="tg-ihln">1</td>
    <td class="tg-0lax">Minimized</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ MAXIMIZE</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Maximized</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ RESTORE</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">When the size is other than maximize / minimize</td>
  </tr>
</tbody>
</table>
        </td>
    </tr>
</table>

<br>**<small>Added since Version 4.1.3</small>**
<br>**<small>Not supported in Mobile, AI</small>**