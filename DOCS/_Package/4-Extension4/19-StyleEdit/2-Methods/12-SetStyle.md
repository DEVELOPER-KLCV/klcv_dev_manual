---
layout: default

grand_parent: StyleEdit Class
parent: Methods
has_children: false
title: StyleEdit.SetStyle Method
nav_order: 12
permalink: /package/extension4/styleedit/methods/setstyle
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Register the style in the style number.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">StyleEdit1.SetStyle( <b><i>styleNo</i></b>, <b><i>fgColor</i></b> [, <b><i>bgColor</i></b> [, <b><i>fontFace</i></b> [, <b><i>fontKind</i></b> [, <b><i>fontSize</i></b> [, <b><i>hotSpot</i></b> ] ] ] ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="7">Arguments</td>
    <td>integer <b><i>styleNo</i></b></td>
    <td>The style number to register. The range is 9 to 30.</td>
  </tr>
  <tr>
    <td>integer <b><i>fgColor</i></b></td>
    <td>Specify the font color with a <a href="/base/color">color constant</a>.</td>
  </tr>
  <tr>
    <td>integer <b>bgColor </b></td>
    <td>Specify the background color with a <a href="/base/color">color constant</a>.</td>
  </tr>
  <tr>
    <td>integer <b><i>fontFace</i></b></td>
    <td>Specifies the decoration attributes of the font. The value follows the FontFace property.</td>
  </tr>
  <tr>
    <td>integer <b><i>fontKind</i> </b></td>
    <td>Specifies the font type. The value follows the FontKind property.</td>
  </tr>
  <tr>
    <td>integer <b><i>fontSize</i></b></td>
    <td>Specifies the font size. The value follows the FontSize property.</td>
  </tr>
  <tr>
    <td>boolean <b><i>hotSpot</i></b></td>
    <td>Specify $TRUE if you want to specify hotspot attributes.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>Func-4</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    StyleEdit1.SetStyle(9, $BLUE, $RED, $FIXED, $FONT2, 14, $TRUE);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension4/styleedit/methods/setkeywordstyle">SetKeywordStyle</a>, <a href="/package/extension4/styleedit/methods/resetstyle">ResetStyle</a>  method</td>
  </tr>
</table>
