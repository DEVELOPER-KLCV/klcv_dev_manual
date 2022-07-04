---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.ExpandFold Method
nav_order: 4
permalink: /package/extension4/styleedit/methods/expandfold
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Folds and unfolds between braces. Only valid when the FoldBrace property is $TRUE.<br><small><span style="color:red">Added since Ver.4.1.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">StyleEdit1.ExpandFold( <b><i>line</i></b> [, <b><i>expand</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b><i>line</i></b></td>
    <td>Specify the line number starting from 0. <br>The operation is the same regardless of which line between the braces is specified. <br>If -1 is specified, all lines will be targeted.</td>
  </tr>
  <tr>
    <td>boolean <b><i>expand</i></b></td>
    <td>Specify $TRUE to expand between braces and $ FALSE to collapse.<br> If omitted, it will be $TRUE.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid argument</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    StyleEdit1.ExpandFold(10, false);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>