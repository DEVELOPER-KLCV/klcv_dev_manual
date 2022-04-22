---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.FindObject Method
nav_order: 7
permalink: /package/system/object/methods/findobject
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.FindObject( <b>name</b> [, <b>rule</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>name</b> or Class identifier</td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>rule</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td><code><pre>
   /* Search for Form objects from parents or ancestors */
var form_obj = FindObject(Form, FIND_ANCESTOR);
 
/* Search for a function with the same rules as the event handler */
var fnc = FindObject("OnTouch", FIND_EVENTPATH);
if (fnc != null) {
    fnc(e);
}
 
/* Search for txCode in object-scoped rules */
var obj = FindObject("txCode", FIND_SCOPEPATH);
if (obj != null) {
    obj.BgColor = $red;
}
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td><a href="/package/system/object/methods/findchild">FindChild</a> method</td>
  </tr>
</table>



