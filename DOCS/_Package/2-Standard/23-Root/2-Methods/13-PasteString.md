---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.PasteString Property
nav_order: 13
permalink: /package/standard/root/methods/pastestring
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Get the string from the clipboard.<br><br>If the clipboard is locked by another application, or if the clipboard does not contain a string, an empty string is returned.<br><br><small><span style="color:red">Added since Ver.4.1.1, Mobile Ver.3.2.1</span></small><br><small><span style="color:blue">Not supported in AI</span></small>
 </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var t = //.PasteString( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
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
    <td colspan="2">
    <code><pre>
    vat t = //.PasteString();
    print(t, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/copystring">CopyString</a> method</td>
  </tr>
</table>



