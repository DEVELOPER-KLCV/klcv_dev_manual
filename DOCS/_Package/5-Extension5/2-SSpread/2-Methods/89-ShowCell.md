---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ShowCell Method
nav_order: 89
permalink: /package/extension5/sspread/methods/showcell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ShowCell(<b>col</b>, <b>row</b>, <b>position</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>position</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    if (!IsVisible(10, 10, $FALSE)) {
        ShowCell(10, 10, $PositionUpperLeft);
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/leftcol">LeftCol</a>, <a href="/package/extension5/sspread/properties/toprow">TopRow</a> properties<br><a href="/package/extension5/sspread/methods/getbottomrightcell">GetBottomRightCell</a>, <a href="/package/extension5/sspread/methods/setactivecell">SetActiveCell</a> methods<br><a href="/package/extension5/sspread/events/topleftchange">TopLeftChange</a> event</td>
  </tr>
</table>
