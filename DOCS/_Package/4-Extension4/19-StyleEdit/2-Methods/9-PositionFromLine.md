---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.PositionFromLine Method
nav_order: 9
permalink: /package/extension4/styleedit/methods/positionfromline
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Find the position of the first character of a line from the line number.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var pos = StyleEdit1.PositionFromLine( <b><i>line</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">integer character position<br>※ Always -1 during object initialization</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>line</i></b></td>
    <td>Specify the line number starting from 0.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var pos = StyleEdit1.PositionFromLine(1);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/styleedit/methods/linefromposition">LineFromPosition</a> method</td>
  </tr>
</table>