---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetRefStyle Method
nav_order: 46
permalink: /package/extension5/sspread/methods/getrefstyle
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetRefStyle()</td>
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
    var ret = GetRefStyle();
    var style = "";
    switch (ret) {
        case $RefStyleDefault:
            style = "Default";
            break;
        case $RefStyleA1:
            style = "A1";
            break;
        case $RefStyleR1C1:
            style = "R1C1";
            break;
    }
    MessageBox("The reference style is " + style + " style");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/formula">Formula</a> property<br><a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a>, <a href="/package/extension5/sspread/methods/setrefstyle">SetRefStyle</a> methods</td>
  </tr>
</table>
