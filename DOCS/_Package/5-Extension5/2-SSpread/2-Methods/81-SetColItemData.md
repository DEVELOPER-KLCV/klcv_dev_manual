---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetColItemData Method
nav_order: 81
permalink: /package/extension5/sspread/methods/setcolitemdata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sets individual numeric data for the specified column. <br><br> Use the GetColItemData method to get individual numeric data for a column. This numeric data does not affect the behavior of the spreadsheet. It can be used for any purpose.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetColItemData(<b>col</b>, <b>value</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Column index</td>
  </tr>
  <tr>
    <td><b>value</b></td>
    <td>Numerical data</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>The argument of SetColItemData is invalid</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the SetColItemData method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/celltag">CellTag</a> property<br><a href="/package/extension5/sspread/methods/getcolitemdata">GetColItemData</a>, <a href="/package/extension5/sspread/methods/getrowitemdata">GetRowItemData</a>, <a href="/package/extension5/sspread/methods/setrowitemdata">SetRowItemData</a> methods</td>
  </tr>
</table>
