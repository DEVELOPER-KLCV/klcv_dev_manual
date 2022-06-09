---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.GetPowerState Property
nav_order: 31
permalink: /package/standard/root/methods/getpowerstate
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the AC Power and battery status.<br><small><span style="color:red">Can only be used with Mobile and AI<br>Only supported since Mobile Ver.3.2.1, AI Ver.1.0.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var state = //.GetPowerState( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a Record object with the following child objects :<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-4erg{border-color:inherit;font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-7jy7{background-color:#D9D9D9;border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-xqm4{background-color:#D9D9D9;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-6t3r{font-style:italic;font-weight:bold;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7jy7">Type</th>
    <th class="tg-7jy7">Name</th>
    <th class="tg-xqm4">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-4erg">ACPower</td>
    <td class="tg-0lax">-1: Unknown, 0: No power connection, 1: Power connection</td>
  </tr>
  <tr>
    <td class="tg-0pky">Number</td>
    <td class="tg-4erg">BatteryLifeLevel</td>
    <td class="tg-0lax">-1: unknown, 0 ( minimum ) to 100 ( maximum )</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-6t3r">BatteryLifeTime</td>
    <td class="tg-0lax">-1: Unknown, 0 or more : Time remaining ( seconds )</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    var state = //.GetPowerState();
    if (state.BatteryLifeLevel >= 0) {
        print("Battery level ", state.BatteryLifeLevel, "%\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



