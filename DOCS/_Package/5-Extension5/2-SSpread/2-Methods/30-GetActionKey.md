---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetActionKey Method
nav_order: 30
permalink: /package/extension5/sspread/methods/GetActionKey
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetActionKey(<b>action</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>action</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var ret = GetActionKey($ActionKeyClear);
    var keyDesc = "";
    if (ret.Shift == $TRUE) {
        keyDesc += "Shift + ";
    }
    if (ret.Ctrl == $TRUE) {
        keyDesc += "Ctrl + ";
    }
    keyDesc += "Virtual key code:" + str(ret.Key);
    MessageBox("Data erasure of active cell is associated with " + keyDesc);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/setActionKey">SetActionKey</a> method</td>
  </tr>
</table>
