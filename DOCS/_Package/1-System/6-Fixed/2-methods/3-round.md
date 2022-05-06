---
layout: default

grand_parent: Fixed Class
parent: Methods
has_children: false
title: Fixed.Round method
nav_order: 3
permalink: /package/system/fixed/methods/Round
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns the rounded object of the specified parameter as a Fixed object.<br>This method is a static method. It can be called without creating an object.<br>The rounding of the Fixed.Round method (when the number of digits = 0) is the maximum (positive direction) of the integers of the value +0.5 or less.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var f = Fixed.Round ( <b>n [, d ]</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Rounded value ( Fixed object)</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>n</b></td>
    <td>Specify the number to be rounded as Fixed type, Number type, or String type.</td>
  </tr>
  <tr>
    <td>integer <b>d</b></td>
    <td>Specify the digit you want to round.<br>It can be specified by -14 to 3. <br>0 is rounded to the nearest whole number, and 3 is rounded to the third decimal place.<br> If it is a negative number, it will be specified in the direction of the integer value. If omitted, it is 0. </td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print (Fixed.Round (12345.678F, -2)); / * 12300 * /
print (Fixed.Round (12345.678F));      / * It becomes 12346 * /
print (Fixed.Round (12345.678F, 2));   / * It becomes 12345.68 * /
 
print (Fixed.Round (0.49F));   / * 0 * /
print (Fixed.Round (0.50F));   / * 1 * /
print (Fixed.Round (0.51F));   / * 1 * /
print (Fixed.Round (-0.49F)); / * 0 * /
print (Fixed.Round (-0.50F)); / * 0 * /
print (Fixed.Round (-0.51F)); / * -1 * /</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



