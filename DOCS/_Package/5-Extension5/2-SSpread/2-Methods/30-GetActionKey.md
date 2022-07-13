---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetActionKey Method
nav_order: 30
permalink: /package/extension5/sspread/methods/getactionkey
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the shortcut key associated with a particular action.<br><br>Use the <a href="/package/extension5/sspread/methods/setactionkey">SetActionKey</a> method if you want to associate a shortcut key with a particular action.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetActionKey(<b>action</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-pf8i{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;
  text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Type</th>
    <th class="tg-cqgq">Name</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Shift</td>
    <td class="tg-j5n6">Shift key state ( $TRUE or $FALSE )</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Ctrl</td>
    <td class="tg-j5n6">[ Ctrl ] key state ( $TRUE or $FALSE )</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Key</td>
    <td class="tg-0lax">The key associated with a particular action</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>action</b></td>
    <td>Actions for which you want to find out the shortcut key <br>Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-pf8i{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;
  text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Type</th>
    <th class="tg-cqgq">Name</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Shift</td>
    <td class="tg-j5n6">Shift key state ( $TRUE or $FALSE )</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Ctrl</td>
    <td class="tg-j5n6">[ Ctrl ] key state ( $TRUE or $FALSE )</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Key</td>
    <td class="tg-0lax">The key associated with a particular action</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of GetActionKey is invalid.</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the GetActionKey method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetActionKey($ActionKeyClear);
    var keyDesc = "";
    if (ret.Shift == $TRUE) {
        keyDesc += "Shift + ";
    }
    if (ret.Ctrl == $TRUE) {
        keyDesc += "Ctrl + ";
    }
    keyDesc += "Virtual key code:" + str(ret.Key);
    MessageBox("Data erasure of active cell is associated with " + keyDesc);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/setactionkey">SetActionKey</a> method</td>
  </tr>
</table>
