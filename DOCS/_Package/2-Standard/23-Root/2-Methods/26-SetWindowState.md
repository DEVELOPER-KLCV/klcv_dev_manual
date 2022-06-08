---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetWindowState Property
nav_order: 26
permalink: /package/standard/root/methods/setwindowstate
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Maximize and minimize the root window and change the context.<br><small><span style="color:red">Added since Ver.4.1.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small><br><br>Specify the size status with one of the values ​​below.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetWindowState( <b>state</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>state</b></td>
    <td>Specify the window size settings and the context settings.<br>If both are specified at the same time, the values will be added. ($ MAXMIZE + $ FRONT, etc.)<br><br>Specify the size status with one of the values below.<style type="text/css">
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
    <td class="tg-0pky">$ MINIMIZE</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Minimize</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ MAXIMIZE</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">Maximize</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ RESTORE</td>
    <td class="tg-c3ow">3</td>
    <td class="tg-0pky">If it is currently maximized or minimized, restore it.</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ FULLSCREEN</td>
    <td class="tg-c3ow">32</td>
    <td class="tg-0pky">Moves to full screen display mode without title bar.<br><small><span style="color:red">Added since Ver.5.0.2</span></small></td>
  </tr>
</tbody>
</table><br><br>Specify the context with one of the values ​​below.<br><style type="text/css">
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
    <td class="tg-0pky">$ FRONT</td>
    <td class="tg-c3ow">8</td>
    <td class="tg-0pky">Move the window to the front</td>
  </tr>
  <tr>
    <td class="tg-0pky">$ BACK</td>
    <td class="tg-c3ow">16</td>
    <td class="tg-0pky">Move the window to the back</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetWindowState($MAXIMIZE + $FRONT);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/events/windowstatechanged">WindowStateChanged</a> event</td>
  </tr>
</table>



