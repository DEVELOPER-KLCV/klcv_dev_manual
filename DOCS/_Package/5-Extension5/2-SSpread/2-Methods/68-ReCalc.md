---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.OpenExcel2007File Method
nav_order: 68
permalink: /package/extension5/sspread/methods/OpenExcel2007File
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
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
    <td></td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a>, <a href="/package/extension5/sspread/properties/formula">Formula</a> properties<br><a href="/package/extension5/sspread/methods/ReCalcCell">ReCalcCell</a> method</td>
  </tr>
</table>
