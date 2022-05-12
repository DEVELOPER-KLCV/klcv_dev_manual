---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ClipboardCopy Method
nav_order: 5
permalink: /package/extension5/sspread/methods/clipboardcopy
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ClipboardCopy()</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function OnRClicked(e) {
        var ret = PopupMenu("Copy", "Cut", "Paste");
        switch (ret) {
        case 1:
            ClipboardCopy();
            break;
        case 2:
            ClipboardCut();
            break;
        case 3:
            ClipboardPaste();
            break;
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/clipboardoptions">ClipboardOptions</a> property<br><a href="/package/extension5/sspread/methods/clipboardcut">ClipboardCut</a>, <a href="/package/extension5/sspread/methods/clipboardpaste">ClipboardPaste</a> methods</td>
  </tr>
</table>
