---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.EditError Event
nav_order: 24
permalink: /package/extension5/sspread/events/editerror
---
# {{ page.title }}

Occurs when an invalid input operation is performed.

The following child objects are attached to the Event object.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-pf8i{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;font-style:italic;font-weight:bold;
  text-align:center;vertical-align:top}
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
    <td class="tg-j5n6">Column number of the cell where the invalid input was made</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">Row</td>
    <td class="tg-j5n6">Row number of the cell where the invalid input was made</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">EditError</td>
    <td class="tg-j5n6">Integer value corresponding to the operation performed<br>The following values are set.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-pnam{border-color:inherit;color:#000000;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-z50u">Value</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Type in a locked cell</td>
  </tr>
  <tr>
    <td class="tg-lcf4">2</td>
    <td class="tg-pnam">When the value of the <a href="/package/extension5/sspread/properties/restrictcols">RestrictCols</a> property is $TRUE , enter one or more columns apart.</td>
  </tr>
  <tr>
    <td class="tg-lcf4">3</td>
    <td class="tg-pnam">When the value of the <a href="/package/extension5/sspread/properties/restrictrows">RestrictRows</a> property is $TRUE, enter one or more rows apart.</td>
  </tr>
  <tr>
    <td class="tg-lcf4">4</td>
    <td class="tg-pnam">When the value of each property of <a href="/package/extension5/sspread/properties/restrictcols">RestrictCols</a> and <a href="/package/extension5/sspread/properties/restrictrows">RestrictRows</a> is $TRUE, enter one or more columns and one or more rows apart.</td>
  </tr>
  <tr>
    <td class="tg-lcf4">5</td>
    <td class="tg-j5n6">Make an invalid entry in a cell and move to another cell</td>
  </tr>
  <tr>
    <td class="tg-lcf4">9</td>
    <td class="tg-j5n6">Enter an invalid key in a check box type cell</td>
  </tr>
</tbody>
</table></td>
  </tr>
</tbody>
</table>

Example of usage<br>
```
Function OnEditError(e) {
    if (e.EditError == 1) {
        MessageBox (strf ("(% 1,% 2) is locked ", e.Col, e.Row));
    }
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/lock">Lock</a>, <a href="/package/extension5/sspread/properties/protect">Protect</a>, <a href="/package/extension5/sspread/properties/restrictcols">RestrictCols</a>, <a href="/package/extension5/sspread/properties/restrictrows">RestrictRows</a> property <br><a href="/package/extension5/sspread/events/editchange">EditChange</a>, <a href="/package/extension5/sspread/events/editmodeoff">EditModeOff</a>, <a href="/package/extension5/sspread/events/editmodeon">EditModeOn</a> event
