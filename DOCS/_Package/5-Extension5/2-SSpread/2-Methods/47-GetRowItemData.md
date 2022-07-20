---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetRowItemData Method
nav_order: 47
permalink: /package/extension5/sspread/methods/getrowitemdata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the individual numeric data set in the specified row.<br><br> Use the <a href="/package/extension5/sspread/methods/setrowitemdata">SetRowItemData</a> method to set individual numeric data for a row. <br>This numeric data does not affect the behavior of the spreadsheet. It can be used for any purpose.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetRowItemData(<b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Numerical data<br>0 is returned for rows that are not set.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>row</b></td>
    <td>Row number</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltag">CellTag</a> property<br><a href="/package/extension5/sspread/methods/getcolitemdata">GetColItemData</a>, <a href="/package/extension5/sspread/methods/setcolitemdata">SetColItemData</a>, <a href="/package/extension5/sspread/methods/setrowitemdata">SetRowItemData</a> methods</td>
  </tr>
</table>
