---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.BeforeEditMode Event
nav_order: 8
permalink: /package/extension5/sspread/events/beforeeditmode
---
# {{ page.title }}

Occurs just before the edit mode starts.

The following child objects are attached to the Event object.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-i7zr{font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-pf8i{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;
  text-align:center;vertical-align:top}
.tg .tg-ux05{font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;text-align:center;
  vertical-align:top}
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
    <td class="tg-pf8i">Col</td>
    <td class="tg-j5n6">Column number of the cell that switches to edit mode</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Row</td>
    <td class="tg-j5n6">Row number of cell to switch to edit mode</td>
  </tr>
  <tr>
    <td class="tg-i7zr">Number</td>
    <td class="tg-ux05">UserAction</td>
    <td class="tg-i7zr">User action<br>The following values are set.<br>
    <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-tcrt{font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-i7zr{font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Constant</th>
    <th class="tg-cqgq">Value</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$BeforeEditModeKeyboard</td>
    <td class="tg-lcf4">0</td>
    <td class="tg-j5n6">Switch to edit mode by key operation</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$BeforeEditModeMouse</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Switch to edit mode by operating the mouse</td>
  </tr>
  <tr>
    <td class="tg-i7zr">$BeforeEditModeCode</td>
    <td class="tg-tcrt">2</td>
    <td class="tg-i7zr">Switch to edit mode by code</td>
  </tr>
</tbody>
</table></td>
  </tr>
</tbody>
</table>

The <a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a> event is fired when the edit mode starts, and the <a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a> event is fired when the edit mode is finished.

Example of usage

```
Function OnBeforeEditMode (e) {
    var what;
    switch (e.UserAction) {
        case $ BeforeEditModeKeyboard:
            what = " key operation ";
            break;
        case $ BeforeEditModeMouse:
            what = " mouse operation ";
            break;
        case $ BeforeEditModeCode:
            what = " code ";
            break;
    }
    print (e.Col, e.Row, what, "\ n");
}
```

Related Item<br>
<a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a>,  <a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a> event
