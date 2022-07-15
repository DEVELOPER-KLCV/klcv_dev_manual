---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ReCalc Method
nav_order: 68
permalink: /package/extension5/sspread/methods/recalc
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"> Recalculate the formula for the entire spreadsheet.<br><br>Use this method to recalculate all formulas in your spreadsheet when the <a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a> property is set to $FALSE.<br><br> Use the <a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a> method to recalculate the formulas in individual cells.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ReCalc()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td>An error occurred in the ReCalc method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    AutoCalc = $FALSE;
    Function OnEditModeOff(e) {
        if (e.ChangeMade) {
            ReCalc();
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a>, <a href="/package/extension5/sspread/properties/formula">Formula</a> properties<br><a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a> method</td>
  </tr>
</table>
