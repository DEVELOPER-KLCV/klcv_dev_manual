---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.ClipboardCut Method
nav_order: 6
permalink: /package/extension5/sspread/methods/clipboardcut
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Copies the selected cell block to the clipboard. <br><br>When exchanging data via the clipboard, use the tab-separated text format. If no cell is selected, the active cell is copied. Use the <a href="/package/extension5/sspread/properties/clipboardoptions">ClipboardOptions</a> property to change the handling of headers in clipboard operations.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">ClipboardCut()</td>
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
    <td>An error occurred in the ClipboardCopy method</td>
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/clipboardoptions">ClipboardOptions</a> property<br><a href="/package/extension5/sspread/methods/clipboardcopy">ClipboardCopy</a>, <a href="/package/extension5/sspread/methods/clipboardpaste">ClipboardPaste</a> methods</td>
  </tr>
</table>
