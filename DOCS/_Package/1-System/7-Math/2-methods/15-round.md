---
layout: default

grand_parent: Math Class
parent: Methods
has_children: false
title: Math.round methods
nav_order: 15
permalink: /package/system/math/methods/round
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Find the value rounded to the nearest whole number.<br>Returns the integer closest to the value ( value + the largest (positive direction) of integers less than or equal to 0.5 )</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var v = Math.round  (<b>x</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns an integer rounded to the nearest whole number.</td>
  </tr>  
 <tr>
    <td>Arguments</td>
    <td>Number <b>x</b></td>
    <td>Value to round off to the nearest whole number</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>print (Math.round (0.49), "￥ n");   / * 0 * /
print (Math.round (0.50), "￥ n");   / * 1 * /
print (Math.round (0.51), "￥ n");   / * 1 * /
 
print (Math.round (-0.49), "￥ n"); / * 0 * /
print (Math.round (-0.50), "￥ n"); / * 0 * /
print (Math.round (-0.51), "￥ n"); / * -1 * /</code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/math/methods/ceil">ceil </a>, <a href="/package/system/math/methods/floor">floor</a> methods</td>
  </tr>
</table>



