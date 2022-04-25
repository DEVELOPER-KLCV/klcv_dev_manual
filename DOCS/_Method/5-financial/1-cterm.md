---
layout: default

parent: Financial Functions

title: cterm
nav_order: 1
permalink: /method/financial/cterm
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"><b>Find the period during which the principal</b> reaches the <b>target maturity amount.</b></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var c = cterm (<b>interest, target maturity, principal </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns the period (year) until the <b>target maturity is reached when the principal</b> is invested at the interest rate.</td>
  </tr>  
   <tr>
    <td rowspan="3">Arguments</td>
    <td>Number  <b>interest</b></td>
    <td>For 5% , specify 0.05</td>
  </tr>
  <tr>
    <td>Number  <b>Target maturity amount</b></td>
    <td>Target amount</td>
  </tr>
  <tr>
    <td>Number <b>Principal</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var a = cterm (0.05, 1000000, 800000);
/ * a is the number of years to operate 800,000 principal at an annual rate of 5 % to 1 million * /</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





