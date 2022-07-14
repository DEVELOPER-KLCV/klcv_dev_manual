---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.IsVisible Method
nav_order: 58
permalink: /package/extension5/sspread/methods/isvisible
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns whether the specified cell, row, or column is displayed within the display area of the spreadsheet.<br><br>Specify -1 for the argument <b>col</b> to specify only the <b>row</b>, and -1 for the argument row to specify only the column. However, only rows or columns are specified, the argument <b>partial</b> is invalid, and if only a part is displayed, $TRUE is returned.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">IsVisible(<b>col</b>, <b>row</b>, <b>partial</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$TRUE if the cell is visible, $FALSE if it is not visible</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td>Cell column position</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Cell row position</td>
  </tr>
  <tr>
    <td><b>partial</b></td>
    <td>$TRUE to see only partially visible cells, $FALSE to see all visible cells</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    if (IsVisible(5, 10, $TRUE) == $TRUE) {
        MessageBox("(5, 10) is displayed");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
</table>
