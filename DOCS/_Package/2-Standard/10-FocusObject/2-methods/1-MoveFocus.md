---
layout: default

grand_parent: FocusObject Class
parent: Methods
has_children: false
title: FocusObject.MoveFocus Method
nav_order: 1
permalink: /package/standard/focusObject/methods/movefocus
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.MoveFocus( [ <b>direction</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>direction</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
if (MessageBox("確認してください", "確認", $OkCancel) == OkSelected) {
    TextBox1.MoveFocus($PREVFOCUS);
}
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



