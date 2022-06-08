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
    <td colspan="2">Register the key in Biz / Browser and get the internal key ID.<br>This key ID can be used to specify keys such as the AltKey and NextTabKey properties.<br><br>An error will occur if you specify a combination of keys that has already been registered.<br><br>The specification is valid until you log out.<br><small><span style="color:red">Added since Ver.5.0.3</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var keyId = //.RegisterFunctionKey( <b>KeyCode</b> [, <b>shift</b> [, <b>ctrl</b> [, <b>alt</b> ]]] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Biz / Browser internal key ID</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>integer <b>KeyCode</b></td>
    <td>Specify the Windows virtual key code.<br>Please refer to sites such as MSDN for virtual key codes.</td>
  </tr>
  <tr>
    <td>boolean <b>shift</b></td>
    <td>Specify the combination with pressing the Shift key with $ TRUE.<br> If omitted, it is considered as $ FALSE.</td>
  </tr>
  <tr>
    <td>boolean <b>ctrl</b></td>
    <td>Specify the combination with pressing the Ctrl key with $ TRUE.<br> If omitted, it is considered as $ FALSE.</td>
  </tr>
  <tr>
    <td>boolean <b>alt</b></td>
    <td>Specify the combination with pressing the Alt key with $ TRUE.<br> If omitted, it is considered as $ FALSE.</td>
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



