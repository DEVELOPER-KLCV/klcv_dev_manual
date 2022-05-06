---
layout: default

parent: 4. Statistical Functions
title: rank
nav_order: 8
permalink: /method/statistical/rank
---



# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Finds the order of the specified data .</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var  r = rank  ( <b>specified data , order , range </b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Rank within the specified  <b>data range</b> <br> <small><i>Behavior changed since Ver.5.0.2, Mobile Ver.4.5.0, AI Ver 1.0.2-></i></small> <br>Returns -1 if not found in the data</td>
  </tr>  
   <tr>
    <td rowspan="4">Arguments</td>
    <td>Date or Number <b>specified data</b></td>
    <td>Data for ranking</td>
  </tr>
  <tr>
    <td>Number  <b>order</b></td>
    <td> 0: Descending order  1: Ascending order</td>
  </tr>
  <tr>
    <td>Date or Number <b>range</b></td>
    <td>Array object name</td>
  </tr>
  <tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var arr = new Number [20];
for (var n = 0; n <arr.Length; n ++) {
arr [n] = int (rand () * 10);
print (arr [n], "");
}
print (" The value of arr [0] is " + str (arr [0]) + " . The rank is " + str (rank (arr [0], 0, arr)) + " rank ￥ n");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>





