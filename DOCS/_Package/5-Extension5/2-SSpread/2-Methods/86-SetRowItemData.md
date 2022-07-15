---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetRowItemData Method
nav_order: 86
permalink: /package/extension5/sspread/methods/setrowitemdata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set individual numerical data for each specified row. Use the <a href="/package/extension5/sspread/methods/getrowitemdata">GetRowItemData</a> method to get individual numeric data for a row. This numeric data does not affect the behavior of the spreadsheet. It can be used for any purpose.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetRowItemData(<b>row</b>, <b>value</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>row</b></td>
    <td>Row number</td>
  </tr>
  <tr>
    <td><b>value</b></td>
    <td>Numerical data</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of SetRowItemData is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the SetRowItemData method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    SetRowItemData(1, 2001);
    SetRowItemData(2, 2002);
    SetRowItemData(3, 2003);
    Function OnClicked(e) {
        MessageBox(str(GetRowItemData(e.Row)) + " is clicked");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltag">CellTag</a> property<br><a href="/package/extension5/sspread/methods/getcolitemdata">GetColItemData</a>, <a href="/package/extension5/sspread/methods/getrowitemdata">GetRowItemData</a>, <a href="/package/extension5/sspread/methods/setcolitemdata">SetColItemData</a> methods</td>
  </tr>
</table>
 