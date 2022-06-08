---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.CopyString Property
nav_order: 2
permalink: /package/standard/root/methods/copystring
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Copy the string to the clipboard. <br>No copy is done if the clipboard is locked by another application. <br> <i><b>Restrictions on Mobile version</b></i> <br>Characters that are in Unicode but not in Shift-JIS are "?" because the characters are converted from Unicode to Shift-JIS during acquisition. <br><small><span style="color:red">Added since Ver.4.1.1</span></small><br><small><span style="color:blue">Not supported in AI</span></small> </td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.CopyString( <b>text</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>text</b></td>
    <td>Specify the character string to copy</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.CopyString("text data");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/pastestring">PasteString</a> method</td>
  </tr>
</table>



