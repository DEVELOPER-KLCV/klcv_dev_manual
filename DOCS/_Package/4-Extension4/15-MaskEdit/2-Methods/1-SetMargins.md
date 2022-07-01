---
layout: default

grand_parent: MaskEdit Class
parent: Methods
has_children: false
title: MaskEdit.SetMargins Method
nav_order: 1
permalink: /package/extension4/maskedit/methods/setmargins
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the left and right margins. <br>In the initial state, the left and right margins are the OS standard positions.<br><br> When setting the margin, specify that the total value of the left and right margins fits in the character display area of MaskEdit.<br><br><small><span style="color:red">Supported only in AI Ver.1.0.2 or later</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">MaskEdit.SetMargins( <b><i>leftMargin</i></b>, <b><i>rightMargin</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>leftMargin</i></b></td>
    <td>Specify the left margin between 0 and 32767.</td>
  </tr>
  <tr>
    <td>integer <b><i>rightMargin</i></b></td>
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
    MaskEdit1.SetMargins(2, 2);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>