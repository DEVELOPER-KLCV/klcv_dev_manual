---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.HardCopy Property
nav_order: 10
permalink: /package/standard/root/methods/hardcopy
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.HardCopy( [ <b>mode</b> [ , <b>option</b> [ , <b>comment</b> [ , <b>printer</b> ] ] ] ] )<br>OR</br>var img = //.HardCopy( <b>mode</b>, 0, “”, “@image” )<br>**<small>Added since Version 5.0.3</small>**
 </td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="4">Arguments</td>
    <td>integer <b>mode</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>option</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>comment</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>printer</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="6">Exception</td>
    <td>PKG-39</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-40</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-41</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-42</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-43</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-44</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.HardCopy($HC_FORM, $HC_VERSION + $HC_COMMENT, "TEST", null);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



