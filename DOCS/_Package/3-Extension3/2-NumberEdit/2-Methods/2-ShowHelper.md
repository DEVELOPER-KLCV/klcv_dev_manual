---
layout: default

grand_parent: NumberEdit Class
parent: Methods
has_children: false
title: NumberEdit.ShowHelper Method
nav_order: 2
permalink: /package/extension3/numberedit/methods/showhelper
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Display a simple calculator.<br><br>It cannot be used before the NumberEdit object is displayed on the screen. Please call after the screen is displayed.<br><br><small><span style="color:red">Added since Ver.4.2.0, Mobile Ver.3.0.0</span></small> <br><small><span style="color:blue">Not supported in AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">NumberEdit1.ShowHelper( [ <b><i>d</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b><i>d</i></b></td>
    <td>Specify the initial value to be displayed on the calculator. If omitted, 0 is displayed.<br><small><span style="color:blue">Not supported in Mobile</span></small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    NumberEdit1.ShowHelper(5000);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>
