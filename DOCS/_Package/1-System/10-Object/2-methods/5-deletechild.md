---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.DeleteChild Method
nav_order: 5
permalink: /package/system/object/methods/deletechild
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td>Disconnects all child objects connected to the object from the object tree.<br><br>See the <a href="/package/system/object/methods/delete">Delete</a> method for disconnecting from the object tree.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.DeleteChild( )</td>
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
    <td><code><pre>Function OnTouch(e) {
    //.Form1.DeleteChild();
    //.Form1.Get("Form1Sub.crs");
}
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td><a href="/package/system/object/methods/delete">Delete</a>, <a href="/package/system/object/methods/append">Append</a> methods</td>
  </tr>
</table>



