---
layout: default

grand_parent: EditBox Class
parent: Methods
has_children: false
title: EditBox.SetSelection Method
nav_order: 3
permalink: /package/standard/editbox/methods/setselection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the cursor position and selection range.<br>If you have a run-time focus, the specifications take effect immediately.<br><small><span style="color:green">Extension after Ver.5.0.2</span></small><br>If there is no focus at the time of execution, it will be in the execution reserved state and the specification will be reflected when the focus is acquired.<br><small><span style="color:red">Added since Ver.5.0.0</span><br><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">EditBox1.SetSelection( <b>pos</b> [, <b>length</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>pos</b></td>
    <td>Specify the cursor position starting from 0.<br>It will be corrected within the range, when specified outside the range. <br>For non-UString, if a byte boundary of a double-byte character is specified, it is corrected to the previous byte.</td>
  </tr>
  <tr>
    <td>integer <b>length</b></td>
    <td>Specify the selected character length. If omitted, it will be 0 (no selection).<br><br>Special specifications<br><code><pre>SetSelection (0, -1) Select all
SetSelection (-1) Deselection</pre></code></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
EditBox1.SetSelection(1, 4);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/editbox/methods/getselection">GetSelection</a> method</td>
  </tr>
</table>