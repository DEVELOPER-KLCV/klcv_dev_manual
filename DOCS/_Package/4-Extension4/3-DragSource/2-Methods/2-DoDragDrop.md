---
layout: default

grand_parent: DragSource Class
parent: Methods
has_children: false
title: DragSource.DoDragDrop Method
nav_order: 2
permalink: /package/extension4/dragsource/methods/dodragdrop
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Start drag & drop.<br><br>When this method is executed, it waits for the mouse to move for a certain period of time, and if it does not move, the method ends as it is. Also, if the transfer data is not set in advance, it will end as it is.<br><br>When this method is completed, all the data set by the <a href="/package/extension4/dragsource/methods/setstring">SetString</a> method etc. up to that point will be cleared.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">source.DoDragDrop( [ <b><i>type</i></b> [, <b><i>waitTime</i></b> [, <b><i>margin</i></b> ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b><i>type</i></b></td>
    <td>Drag and drop type. Specify the following values. If omitted, it will be $COPYMODE.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-npz6{background-color:#c0c0c0;border-color:#000000;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-f7v4{background-color:#c0c0c0;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-f7v4">Constant</th>
    <th class="tg-npz6">Value</th>
    <th class="tg-f7v4">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$COPYMODE</td>
    <td class="tg-c3ow">256</td>
    <td class="tg-0pky">Copy mode</td>
  </tr>
  <tr>
    <td class="tg-0pky">$MOVEMODE</td>
    <td class="tg-c3ow">512</td>
    <td class="tg-0pky">Move mode</td>
  </tr>
</tbody>
</table>

How to distinguish between copy mode and move mode processing depends on the implementation of the drop destination.

<br><small><span style="color:green">It is now possible to specify $COPYMODE and $MOVEMODE at the same time since Ver.5.0.0</span></small>

</td>
  </tr>
  <tr>
    <td>integer <b><i>waitTime</i></b></td>
    <td>The waiting time for the drag operation after the method is executed. Able to specify 0 to 1000 (1 second) in millisecond units. If omitted, the setting value of the OS is used.</td>
  </tr>
  <tr>
    <td>integer <b><i>margin</i></b></td>
    <td>The movement width of the mouse to move to the drag motion. Able to specify 0 to 16 in pixel units. If omitted, the setting value of the OS is used.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument value</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    source.SetString("Drag and Drop");
    source.DoDragDrop($MOVEMODE, 10, 8);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>