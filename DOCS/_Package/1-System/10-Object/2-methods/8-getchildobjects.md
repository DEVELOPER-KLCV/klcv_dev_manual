---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.GetChildObjects Method
nav_order: 8
permalink: /package/system/object/methods/getchildobjects
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.GetChildObjects( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td><code><pre>
Function setData(objName, objValue) {
    var ca = GetChildObjects();
    if (ca[objName] != null) {
        if (ca[objName].Value != null) {
            ca[objName].Value = objValue;
        }
    }
}
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td><a href="/package/system/object/methods/findchild">FindChild</a> method</td>
  </tr>
</table>



