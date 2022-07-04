---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.GetFoldLevel Method
nav_order: 5
permalink: /package/extension4/styleedit/methods/getfoldlevel
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Find the nesting level of the brace of the target row. If the target line is collapsed, it will be returned as a negative value.<br><small><span style="color:red">Added since Ver.4.1.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var level = StyleEdit1.GetFoldLevel( <b><i>line</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>line</i></b></td>
    <td>Specify the line number starting from 0.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid arguments</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var level = StyleEdit1.GetFoldLevel(100);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>