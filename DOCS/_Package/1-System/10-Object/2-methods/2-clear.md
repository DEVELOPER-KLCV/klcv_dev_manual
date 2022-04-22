---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.Clear Method
nav_order: 2
permalink: /package/system/object/methods/clear
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.Clear( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td>None</td>
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
Function OnTouch(e) {
    var childArray = GetChildObjects();
    for (var i in childArray) {
        childArray[i].Clear();
    }
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td><a href="/package/system/object/methods/clearchild">ClearChild</a> methods</td>
  </tr>
</table>



