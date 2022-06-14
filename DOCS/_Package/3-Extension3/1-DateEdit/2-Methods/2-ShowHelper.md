---
layout: default

grand_parent: DateEdit Class
parent: Methods
has_children: false
title: DateEdit.ShowHelper Method
nav_order: 2
permalink: /package/extension3/dateedit/methods/showhelper
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Display the calendar.<br><br>Not available before the DateEdit object appears on the screen. Call after displaying the screen.<br><br><small><span style="color:red">Added since Ver.4.2.0, Mobile Ver.3.0.0</span></small> <br><small><span style="color:blue">Not supported in AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">DateEdit1.ShowHelper( [ <b><i>d</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b><i>d</i></b></td>
    <td>Specify the initial date to be displayed on the calendar as a character string. If omitted, the current date of the DateEdit object is displayed.<br><small><span style="color:blue">Not supported in AI</span></small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    DateEdit1.ShowHelper("2007/8/30");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>
