---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.LineFromPosition Method
nav_order: 8
permalink: /package/extension4/styleedit/methods/linefromposition
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Find the line number from the text position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var line = StyleEdit1.LineFromPosition( <b><i>pos</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Line number starting with integer 0<br>※ Always -1 during object initialization</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>pos</i></b></td>
    <td>Specify the text position.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var line = StyleEdit1.LineFromPosition(100);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/styleedit/methods/positionfromline">PositionFromLine</a> method</td>
  </tr>
</table>