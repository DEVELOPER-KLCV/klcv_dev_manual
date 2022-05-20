---
layout: default

grand_parent: FocusObject Class
parent: Methods
has_children: false
title: FocusObject.SetFocus Method
nav_order: 2
permalink: /package/standard/focusobject/methods/setfocus
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Set the keyboard focus on the object.<br><br>The focus does not move immediately when I execute the SetFocus method.<br>The object is changed to preferentially receive focus and is set to focus after the ongoing processing is complete.<br><br>If the SetFocus method is executed on multiple objects at once in the same screen, the last executed SetFocus method will be effective.<br><br>Not valid if the object is in a state where it cannot receive focus. <br> <br><small><span style="color:green">Changed since Ver.4.0.2, Mobile Ver.3.0.0 to enable the last setFocus method executed in multiple executions in the same screen.</span></small>
 </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.SetFocus( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
if (MessageBox("確認してください", "確認", $OkCancel) == OkSelected) {
    TextBox1.SetFocus();
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>




