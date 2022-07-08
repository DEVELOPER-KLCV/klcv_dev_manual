---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.BeforeUserSort Event
nav_order: 10
permalink: /package/extension5/sspread/events/beforeusersort
---
# {{ page.title }}

Occurs when sorting data.

※ Sorting has not been completed when this event occurs. Use the <a href="/package/extension5/sspread/events/afterusersort">AfterUserSort</a> event to perform processing that is expected to be performed after sorting is completed.

- User clicks column header

- Set $ColUserSortIndicatorAscending (sort / ascending order) and $ColUserSortIndicatorDescending (sort / descending order) in the <a href="/package/extension5/sspread/properties/colusersortindicator">ColUserSortIndicator</a> property.

- Set $UserColActionSort (sort / indicator display) and $UserColActionSortNoIndicator (sort / indicator hidden) in the <a href="/package/extension5/sspread/properties/usercolaction">UserColAction</a>  property.

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
    <td class="tg-j5n6">Column number of the column to be sorted</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Number</td>
    <td class="tg-pf8i">State</td>
    <td class="tg-j5n6">The type of sort that was performed last time<br>The following values are set.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-cqgq{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
.tg .tg-lcf4{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Constant</th>
    <th class="tg-cqgq">Name</th>
    <th class="tg-0ss8">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">$BeforeUserSortStateNone</td>
    <td class="tg-lcf4">0</td>
    <td class="tg-j5n6">No sorting</td>
  </tr>
  <tr>
    <td class="tg-j5n6">$BeforeUserSortStateAcending</td>
    <td class="tg-lcf4">1</td>
    <td class="tg-j5n6">Sort in ascending order</td>
  </tr>
  <tr>
    <td class="tg-0lax">$BeforeUserSortStateDescending</td>
    <td class="tg-baqh">2</td>
    <td class="tg-0lax">Sort in descending order</td>
  </tr>
</tbody>
</table></td>
  </tr>
</tbody>
</table>

Example of usage<br>

```
Function OnBeforeUserSort (e) {
    var sortDescription;
    switch (e.State) {
        case $ BeforeUserSortStateNone:
            sortDescription = " Not sorted ";
            break;
        case $ BeforeUserSortStateAcending:
            sortDescription = " It was sorted in ascending order ";
            break;
        case $ BeforeUserSortStateDescending:
            sortDescription = " It was sorted in descending order ";
            break;
    }
    MessageBox (str (e.Col) + " column is " + sortDescription);
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/colusersortindicator">ColUserSortIndicator</a>, <a href="/package/extension5/sspread/properties/usercolaction">UserColAction</a> property <br> <a href="/package/extension5/sspread/events/afterusersort">AfterUserSort</a> event 