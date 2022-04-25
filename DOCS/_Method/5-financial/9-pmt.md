---
layout: default

parent: Financial Functions

title: pmt
nav_order: 9
permalink: /method/financial/pmt
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"> Find the repayment amount for each term when the <b>borrowing amount</b> is borrowed at the <b>interest rate</b> with the equal repayment of principal and interest for the <b>number of repayments</b>. For monthly repayments, the <b>interest rate</b> specifies the monthly interest rate as a decimal.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">	var p = pmt (<b>borrowing amount, interest rate, repayment frequency, payment date </b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">The repayment amount for each term is returned when the <b>borrowed amount</b> is borrowed at the <b>interest rate</b> with the equal repayment of the principal and interest of the <b>number of repayments</b>.</td>
  </tr>  
   <tr>
    <td rowspan="4">Arguments</td>
    <td>Number  <b>borrowing amount</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Number  <b>interest rate</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Number <b>frequency repayment</b></td>
    <td>Number of repayments.</td>
  </tr>
    <tr>
    <td>Number <b>payment  date</b></td>
    <td>1 for the beginning of the period and 0 for the end of the period. <br>If omitted, payment will be made at the end of the term .</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>





