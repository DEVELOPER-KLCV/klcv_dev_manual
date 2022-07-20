---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetActionKey Method
nav_order: 78
permalink: /package/extension5/sspread/methods/setactionkey
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set a shortcut key to associate with a specific action. <br><br>Shortcut keys are initially set as follows.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-z50u">Key</th>
    <th class="tg-z50u">Virtual key code</th>
    <th class="tg-xt05">Action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh">F2</td>
    <td class="tg-baqh">113</td>
    <td class="tg-0lax">Erase data in active cell</td>
  </tr>
  <tr>
    <td class="tg-baqh">F3</td>
    <td class="tg-baqh">114 </td>
    <td class="tg-0lax">Display the current date and time on a date or time cell</td>
  </tr>
  <tr>
    <td class="tg-baqh">F4</td>
    <td class="tg-baqh">115 </td>
    <td class="tg-0lax">Show pop-up calendar on date cell</td>
  </tr>
</tbody>
</table><br> These actions can be used in cells in input mode.<br><br> This method can disable these actions or assign a different key.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetActionKey(<b>action</b>, <b>shift</b>, <b>ctrl</b>, <b>key</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>action</b></td>
    <td>Action to associate a shortcut key <br> Specify the following values.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Constant</th>
    <th class="tg-z50u">Value</th>
    <th class="tg-xt05">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">$ActionKeyClear</td>
    <td class="tg-baqh">0</td>
    <td class="tg-0lax">Erase data in active cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ActionKeyCurrent</td>
    <td class="tg-baqh">1</td>
    <td class="tg-0lax">Display the current date and time on a date or time cell</td>
  </tr>
  <tr>
    <td class="tg-0lax">$ActionKeyPopup</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Show pop-up calendar on date cell</td>
  </tr>
</tbody>
</table></td>
  </tr>
  <tr>
    <td><b>shift</b></td>
    <td>[Shift] key state ($TRUE or $FALSE)</td>
  </tr>
  <tr>
    <td><b>ctrl</b></td>
    <td>[Ctrl] key state ($TRUE or $FALSE)</td>
  </tr>
  <tr>
    <td><b>key</b></td>
    <td>Key associated with a specific action (any virtual key code can be used)</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of SetActionKey is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the SetActionKey method

</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    SetActionKey($ActionKeyClear, $TRUE, $FALSE, 113); /* SHIFT+F2 */
    SetActionKey($ActionKeyCurrent, $FALSE, $TRUE, 113); /* CTRL+F2 */
    SetActionKey($ActionKeyPopup, $TRUE, $TRUE, 113); /* SHIFT+CTRL+F2 */
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/getactionkey">GetActionKey</a> method</td>
  </tr>
</table>
