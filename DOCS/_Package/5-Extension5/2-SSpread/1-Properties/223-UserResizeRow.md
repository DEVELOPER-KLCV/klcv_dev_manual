---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.UserResizeRow Property
nav_order: 223
permalink: /package/extension5/sspread/properties/userresizerow
---
# {{ page.title }}

Sets whether the width of the column can be changed with the mouse.

Before setting this property, use the <a href="/package/extension5/sspread/properties/userresizerow">Row</a> property to specify the column of interest.

Specify the following values. The initial value is $UserResizeDefault .

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Constant</th>
    <th class="tg-0pky">Value</th>
    <th class="tg-0pky">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$UserResizeDefault</td>
    <td class="tg-0pky">0</td>
    <td class="tg-0pky">Use the setting of the <a href="/package/extension5/sspread/properties/userresize">UserResize</a> property</td>
  </tr>
  <tr>
    <td class="tg-0pky">$UserResizeOn</td>
    <td class="tg-0pky">1</td>
    <td class="tg-0pky">Can be changed</td>
  </tr>
  <tr>
    <td class="tg-0pky">$UserResizeOff</td>
    <td class="tg-0pky">2</td>
    <td class="tg-0pky">Cannot be changed</td>
  </tr>
</tbody>
</table>

This property allows / prohibits column width changes for specific columns.
The entire spreadsheet is set with the <a href="/package/extension5/sspread/properties/userresize">UserResize</a> property.
Each row is set with the <a href="/package/extension5/sspread/properties/userresizecol">UserResizeCol</a> property.

Example of use
```
/ * Prohibit resizing * /
UserResize = $ UserResizeNone;
/ * Resize permission only for the second column * /
Col = 2;
UserResizeCol = $ UserResizeOn;
/ * Resize permission only for the 3rd line * /
Row = 3;
UserResizeRow = $ UserResizeOn;
```

Related item
<a href="/package/extension5/sspread/properties/userresize">UserResize</a> , <a href="/package/extension5/sspread/properties/userresizecol">UserResizeCol</a> property