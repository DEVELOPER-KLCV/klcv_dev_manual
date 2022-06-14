---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: TextBox.GetSelection Method
nav_order: 3
permalink: /package/standard/textbox/methods/getselection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the current cursor position and selection.<br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var n = TextBox1.GetSelection( [ <b><i>lengthMode</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Cursor position or number of selected bytes</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>boolean <b><i>lengthMode</i></b></td>
    <td>Value to get<br> $ FALSE: Get the cursor position<br> $ TRUE: Gets the number of selected bytes (number of characters for UString)<br> The default is $ FALSE.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TextBox1.GetSelection();
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/textbox/methods/setselection">SetSelection</a> method</td>
  </tr>
</table>



