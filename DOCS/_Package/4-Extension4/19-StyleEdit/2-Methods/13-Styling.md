---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.Styling Method
nav_order: 13
permalink: /package/extension4/styleedit/methods/styling
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Apply a style to the characters.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">StyleEdit1.Styling( <b><i>styleNo</i></b>, <b><i>startPos</i></b>, <b><i>endPos</i></b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b><i>styleNo</i></b></td>
    <td>The style number to apply. The range is 0 to 30. It is necessary to define the style in advance with the SetStyle method and SetKeywordStyle method.</td>
  </tr>
  <tr>
    <td>integer <b><i>startPos</i></b></td>
    <td>Specifies the character position where the style will start to be applied. If -1 is specified, it will start from the beginning.</td>
  </tr>
  <tr>
    <td>integer <b><i>endPos</i></b></td>
    <td>Specifies the character position where the style application ends. If -1 is specified, it will be until the end of the sentence.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td>Invalid arguments</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    StyleEdit1.Styling(8, 10, 20);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/styleedit/methods/setstyle">SetStyle</a>, <a href="/package/extension4/styleedit/methods/setkeywordstyle">SetKeywordStyle</a> method</td>
  </tr>
</table>
