---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: TextBox.SetSelection Method
nav_order: 6
permalink: /package/standard/textbox/methods/setselection
---
# {{ page.title }}

<table> 
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the cursor position and selection range.<br>If you have run-time focus, your specifications will take effect immediately.<br><br><small><span style="color:green">Extension since Ver.5.0.2</span></small><br>If there is no focus at the time of execution, it will be in the execution reserved state and the specification will be reflected when the focus is acquired.<br><br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TextBox1.SetSelection( <b><i>pos</i></b> [, <b><i>length</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer  <b><i>pos</i></b></td>
    <td>Specify the cursor position starting from 0.<br>If you specify outside the range, it will be corrected within the range.<br>For other than UString, if the byte boundary of a 2-byte character is specified, it will be corrected to the previous byte.</td>
  </tr>
  <tr>
    <td>integer <b><i>length</i></b></td>
    <td>Specify the selected character length. If omitted, it will be 0 (no selection).<br><br>Unique specifications<br>&nbsp;&nbsp;SetSelection (0, -1) Select all<br>&nbsp;&nbsp;SetSelection (-1) Deselection</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TextBox1.SetSelection(1, 4);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/textbox/methods/getselection">GetSelection</a> method</td>
  </tr>
</table>



