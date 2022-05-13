---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.RegisterFunctionKey Property
nav_order: 16
permalink: /package/standard/root/methods/registerfunctionkey
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var keyId = //.RegisterFunctionKey( <b>KeyCode</b> [, <b>shift</b> [, <b>ctrl</b> [, <b>alt</b> ]]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>integer <b>KeyCode</b></td>
    <td></td>
  </tr>
  <tr>
    <td>boolean <b>shift</b></td>
    <td></td>
  </tr>
  <tr>
    <td>boolean <b>ctrl</b></td>
    <td></td>
  </tr>
  <tr>
    <td>boolean <b>alt</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    Number BSKEY = RegisterFunctionKey(0x8, $TRUE); /* Shift + BackSpace Key */
    Form frmKeyDown {
          X = 0;
          Y = 0;
          Width = 400;
          Height = 300;
          TextBox TextBox1 {
                  X = 8;
                  Y = 16;
                  Width = 336;
                  Height = 24;
                  PrevTabKey = //.BSKEY; /* Shift + Go to the previous item with BackSpace */
          }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



