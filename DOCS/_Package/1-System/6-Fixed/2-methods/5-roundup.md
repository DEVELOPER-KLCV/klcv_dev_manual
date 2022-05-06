---
layout: default

grand_parent: Fixed Class
parent: Methods
has_children: false
title: Fixed.RoundUp method
nav_order: 5
permalink: /package/system/fixed/methods/RoundUp
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the specified parameter rounded up as a Fixed object.<br>This method is a static method. It can be called without creating an object.<br>Rounding up the Fixed.RoundUp method (when the number of digits = 0) is the <b>closest integer in the direction of the larger absolute value (farther from 0).</b></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var f = Fixed.RoundUp ( <b>n [, d ]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Rounded up value ( Fixed object)</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>n</b></td>
    <td>Specify the number to be round up as Fixed type, Number type, or String type.</td>
  </tr>
  <tr>
    <td>integer <b>d</b></td>
    <td>Specify the digit you want to round up.<br>It can be specified by -14 to 3. <br>0 is round up to the nearest whole number, and 3 is round up to the third decimal place.<br> If it is a negative number, it will be specified in the direction of the integer value. If omitted, it is 0. </td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print (Fixed.RoundUp (12345.678F, -2)); / * 12400 * /
print (Fixed.RoundUp (12345.678F));      / * It becomes 12346 * /
print (Fixed.RoundUp (12345.678F, 2));   / * It becomes 12345.68 * /
 
print (Fixed.RoundUp (0.50F));   / * 1 * /
print (Fixed.RoundUp (-0.50F)); / * -1 * /</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>