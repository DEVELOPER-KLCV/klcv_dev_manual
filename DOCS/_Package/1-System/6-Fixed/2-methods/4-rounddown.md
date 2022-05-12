---
layout: default

grand_parent: Fixed Class
parent: Methods
has_children: false
title: Fixed.RoundDown method
nav_order: 4
permalink: /package/system/fixed/methods/rounddown
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the specified parameter truncated as a Fixed object.<br>This method is a static method. It can be called without creating an object.<br>The Fixed.RoundDown method truncation (when the number of digits = 0) is the closest integer in the direction that the absolute value of the value is smaller (closer to 0).</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var f = Fixed.RoundDown ( <b>n [, d ]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Truncated  value ( Fixed object)</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>n</b></td>
    <td>Specify the number to be truncate as Fixed type, Number type, or String type.</td>
  </tr>
  <tr>
    <td>integer <b>d</b></td>
    <td>Specify the digit you want to truncate.<br>It can be specified by -14 to 3. <br>0 is truncates to the nearest whole number, and 3 is truncates after the third decimal place.<br> If it is a negative number, it will be specified in the direction of the integer value. If omitted, it is 0. </td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print (Fixed.RoundDown (12345.678F, -2)); / * 12300 * /
print (Fixed.RoundDown (12345.678F));      / * It becomes 12345 * /
print (Fixed.RoundDown (12345.678F, 2));   / * It becomes 12345.67 * /
 
print (Fixed.RoundDown (0.50F));   / * 0 * /
print (Fixed.RoundDown (-0.50F)); / * 0 * /</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>