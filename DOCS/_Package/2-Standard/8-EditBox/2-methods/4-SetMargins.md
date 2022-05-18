---
layout: default

grand_parent: EditBox Class
parent: Methods
has_children: false
title: EditBox.SetMargins Method
nav_order: 4
permalink: /package/standard/editbox/methods/setmargins
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the left and right margins.<br>In the initial state, the left and right margins are the OS standard positions.<br>When setting the margin, specify that the total value of the left and right margins fits in the character display area of EditBox.<br><small><span style="color:red">Added since Ver.5.0.2</span><br><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">EditBox1.SetMargins( <b>leftMargin</b>, <b>rightMargin</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>leftMargin</b></td>
    <td>Specify the left margin between 0 and 32767.</td>
  </tr>
  <tr>
    <td>integer <b>rightMargin</b></td>
    <td>Specify the right margin between 0 and 32767.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>FUNC-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
EditBox1.SetMargins(2, 2);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>