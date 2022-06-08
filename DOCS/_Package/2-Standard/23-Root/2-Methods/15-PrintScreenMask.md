---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.PrintScreenMask Property
nav_order: 15
permalink: /package/standard/root/methods/printscreenmask
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Masks the screen capture with the PrintScreen key.<br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.PrintScreenMask( <b>flag</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>boolean <b>flag</b></td>
    <td>If $ TRUE is specified, the masked image will be transferred to the clipboard by pressing the PrintScreen key thereafter.<br> Specifying $ FALSE will restore normal operation.<br><small><span style="color:green">Since Ver.5.0.2, if $ TRUE is specified, the screen capture will not be transferred to the clipboard when the PrintScreen key is pressed after that.</span></small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>PKG-55</td>
    <td>Could not occupy the PrintScreen key</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.PrintScreenMask($TRUE);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



