---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.IsCellSelected Method
nav_order: 53
permalink: /package/extension5/sspread/methods/iscellselected
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns if the specified cell is currently selected.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">IsCellSelected(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$TRUE if selected, $FALSE otherwise</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Cell column number</td>
  </tr>
  <tr>
    <td><b>rows</b></td>
    <td>Cell row number</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function OnRClicked(e) {
        if (IsCellSelected(e.Col, e.Row) == $TRUE) {
            MessageBox("Cell is selected");
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
</table>
