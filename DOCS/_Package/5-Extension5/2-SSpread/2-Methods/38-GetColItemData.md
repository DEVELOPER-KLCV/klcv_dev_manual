---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetColItemData Method
nav_order: 38
permalink: /package/extension5/sspread/methods/getcolitemdata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the individual numeric data set for the specified column.<br><br> Use the SetColItemData method to set individual numeric data for a column.<br> This numeric data does not affect the behavior of the spreadsheet. It can be used for any purpose.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetColItemData(<b>col</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Numerical data<br>0 is returned for columns that are not set.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>col</b></td>
    <td>Column index</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    SetColItemData(1, 1001);
    SetColItemData(2, 1002);
    SetColItemData(3, 1003);
    
    Function OnClicked(e) {
        MessageBox(str(GetColItemData(e.Col)) + " is clicked");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltag">CellTag</a> property<br><a href="/package/extension5/sspread/methods/getrowitemdata">GetRowItemData</a>, <a href="/package/extension5/sspread/methods/setcolitemdata">SetColItemData</a>, <a href="/package/extension5/sspread/methods/getrowitemdata">GetRowItemData</a> methods</td>
  </tr>
</table>
