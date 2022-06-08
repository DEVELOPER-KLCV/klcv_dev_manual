---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.GetFocus Property
nav_order: 8
permalink: /package/standard/root/methods/getfocus
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the focused object in the currently displayed form.<br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var obj = //.GetFocus( [ <b>focus</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Return the object that is currently in focus.</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>boolean <b>focus</b></td>
    <td>In the case of $ FALSE, it returns null if it does not actually have the focus of the OS.<br>In the case of $ TRUE, it returns the focus-owned object that Biz / Browser holds internally even if it does not actually have the focus of the OS.<br>If omitted, the operation is $ FALSE.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    var obj = //.GetFocus();
    obj.Title = "Focus Now.";
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/focusObject/methods/setfocus">FocusObject.SetFocus</a> method</td>
  </tr>
</table>



