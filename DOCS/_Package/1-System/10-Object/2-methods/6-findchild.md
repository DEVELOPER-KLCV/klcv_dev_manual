---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.FindChild Method
nav_order: 6
permalink: /package/system/object/methods/findchild
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.FindChild( <b>name</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>name</b> or Class identifier</td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    /* Search by object name */
var child = FindChild("TEST");
if (child != null) {
    child.Value = "Hello";
}
 
/* Search by class */
var form_obj = FindChild(Form);
if (form_obj != null) {
    form_obj.BgColor = $WHITE;
}
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/object/methods/getchildobjects">GetChildObjects</a> method</td>
  </tr>
</table>



