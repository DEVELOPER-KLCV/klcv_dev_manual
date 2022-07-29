---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.UserColAction Property
nav_order: 220
permalink: /package/extension5/sspread/properties/usercolaction
---
# {{ page.title }}

Sets the action to be taken when a column header is clicked.

Specify the following values. The initial value is $UserColActionDefault .

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
    <td class="tg-0pky">$UserColActionDefault</td>
    <td class="tg-c3ow">0</td>
    <td class="tg-0pky">Select a column</td>
  </tr>
  <tr>
    <td class="tg-0pky">$UserColActionSort</td>
    <td class="tg-c3ow">1</td>
    <td class="tg-0pky">Sort (sort indicator display)</td>
  </tr>
  <tr>
    <td class="tg-0pky">$UserColActionSortNoIndicator</td>
    <td class="tg-c3ow">2</td>
    <td class="tg-0pky">Sort (hide sort indicator)</td>
  </tr>
  <tr>
    <td class="tg-0lax">$UserColActionAutoSize</td>
    <td class="tg-baqh">3</td>
    <td class="tg-0lax">Automatically adjust column width</td>
  </tr>
</tbody>
</table>

Specifying $UserColActionSort , $UserColActionSortNoIndicator allows the user to sort by clicking on the column header.
Sorting is done for the entire spreadsheet, keyed by one particular column.
Detailed settings can be made by combining with the <a href="/package/extension5/sspread/properties/colusersortindicator">ColUserSortIndicator</a> property.

If you specify $UserColActionAutoSize , double-clicking the column header will adjust the column width.

Related item
<a href="/package/extension5/sspread/properties/colusersortindicator">ColUserSortIndicator</a> property