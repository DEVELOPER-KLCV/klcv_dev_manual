---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetActiveCell Method
nav_order: 79
permalink: /package/extension5/sspread/methods/setactivecell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the active cell.<br><br> Refer to the <a href="/package/extension5/sspread/properties/activecol">ActiveCol</a> and <a href="/package/extension5/sspread/properties/activerow">ActiveRow</a> properties to refer to the active cell.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetActiveCell(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td>Cell column number</td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td>Cell row number</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the SetActiveCell method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function OnRClicked(e) {
        SetActiveCell(e.Col, e.Row);
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/activecol">ActiveCol</a>, <a href="/package/extension5/sspread/properties/activerow">ActiveRow</a> properties</td>
  </tr>
</table>
