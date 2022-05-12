---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ReCalcCell Method
nav_order: 69
permalink: /package/extension5/sspread/methods/recalccell
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ReCalcCell(<b>col</b>, <b>row</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>col</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    AutoCalc = $FALSE;
    Col = 2;
    Row = 1;
    Formula = "A1";
    Function OnEditModeOff(e) {
        if (e.ChangeMade && e.Col == 1 && e.Row == 1) {
            ReCalcCell(2, 1);
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a>, <a href="/package/extension5/sspread/properties/formula">Formula</a> properties<br><a href="/package/extension5/sspread/methods/recalc">ReCalc</a> method</td>
  </tr>
</table>
