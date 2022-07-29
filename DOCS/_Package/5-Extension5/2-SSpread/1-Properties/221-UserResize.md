---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.UserResize Property
nav_order: 221
permalink: /package/extension5/sspread/properties/userresize
---
# {{ page.title }}
Set whether to allow the mouse to change the column width and row height.

Specify the following values. The initial value is $UserResizeBoth .
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-kg9c{background-color:#D9D9D9;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-8r26{background-color:#D9D9D9;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-kg9c">Constant</th>
    <th class="tg-8r26">Value</th>
    <th class="tg-kg9c">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">$UserResizeNone</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">Column / row size cannot be changed</td>
  </tr>
  <tr>
    <td class="tg-0pky">$UserResizeColumns</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Columns can be resized</td>
  </tr>
  <tr>
    <td class="tg-0pky">$UserResizeRows</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">Row resizing is possible</td>
  </tr>
  <tr>
    <td class="tg-0lax">$UserResizeBoth</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">Column / row size can be changed</td>
  </tr>
</tbody>
</table>

This property sets the settings for the entire spreadsheet.
The <a href="/package/extension5/sspread/properties/userresizecol">UserResizeCol</a> property is used to set each column, and the <a href="/package/extension5/sspread/properties/userresizerow">UserResizeRow</a> property is used to set each row .

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

<a href="/package/extension5/sspread/properties/userresizecol">UserResizeCol</a> , <a href="/package/extension5/sspread/properties/userresizerow">UserResizeRow</a> property