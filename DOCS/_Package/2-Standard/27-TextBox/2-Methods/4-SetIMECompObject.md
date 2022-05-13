---
layout: default

grand_parent: Spread Class
parent: Methods
has_children: false
title: TextBox.SetIMECompObject Method
nav_order: 4
permalink: /package/standard/textbox/methods/setimecompobject
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">TextBox1.SetIMECompObject( <b>obj</b> [, <b>mode</b> [, <b>showRealtime</b> ] ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>TextBox <b>obj</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>mode</b></td>
    <td></td>
  </tr>
  <tr>
    <td>boolean <b>showRealtime</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>PKG-54</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    TextBox TextBoxShow {  /* 自動入力用 */
        X = 8;
        Y = 140;
        Width = 136;
        Height = 24;
    }
    TextBox TextBox1 {  /* IME入力用 */
        X = 8;
        Y = 40;
        Width = 136;
        Height = 24;
        IMEMode = $DHIRA;
        SetIMECompObject(^.TextBoxShow, $DKANA, $TRUE);
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



