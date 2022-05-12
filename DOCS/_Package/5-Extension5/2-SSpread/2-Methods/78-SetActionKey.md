---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.SetActionKey Method
nav_order: 78
permalink: /package/extension5/sspread/methods/setactionkey
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">SetActionKey(<b>action</b>, <b>shift</b>, <b>ctrl</b>, <b>key</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td><b>action</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>shift</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>ctrl</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>key</b></td>
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
    SetActionKey($ActionKeyClear, $TRUE, $FALSE, 113); /* SHIFT+F2 */
    SetActionKey($ActionKeyCurrent, $FALSE, $TRUE, 113); /* CTRL+F2 */
    SetActionKey($ActionKeyPopup, $TRUE, $TRUE, 113); /* SHIFT+CTRL+F2 */
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/methods/getactionkey">GetActionKey</a> method</td>
  </tr>
</table>
