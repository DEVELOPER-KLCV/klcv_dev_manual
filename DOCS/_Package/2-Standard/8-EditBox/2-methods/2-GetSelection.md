---
layout: default

grand_parent: EditBox Class
parent: Methods
has_children: false
title: EditBox.GetSelection Method
nav_order: 2
permalink: /package/standard/editbox/methods/getselection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the current cursor position and selection range.<br><br><small><span style="color:red">Added since Ver.5.0.0</span><br><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var n = EditBox1.GetSelection( [ <b>lengthMode</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Cursor position or number of selected bytes</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>boolean <b>lengthMode</b></td>
    <td>Value to get <br>$ FALSE : Get the cursor position<br>$ TRUE : Gets the number of selected bytes ( number of characters for UString )<br>The default is $ FALSE .</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
EditBox1.GetSelection();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/editbox/methods/setselection">SetSelection</a> method</td>
  </tr>
</table>