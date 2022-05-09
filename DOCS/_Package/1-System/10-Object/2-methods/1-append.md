---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.Append Method
nav_order: 1
permalink: /package/system/object/methods/append
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Connects the specified object to the object tree as a child object.<br><br>Objects connected to the object tree are no longer deleted when the variable scope disappears and can be referenced from the object tree at any time. If you want to keep the object permanently, connect to the object tree. The connected object can be deleted with the <a href="/package/system/object/methods/delete">Delete</a> method.<br><br>Note that connecting many objects to the object tree can be memory inefficient and slow.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.Append( <b>child [, name ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>child</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>name</b></td>
    <td>The name of the child object.<br>It cannot be specified if the <b>child</b> has already been given a name.<br>An exception will be raised if there are objects with the same name in the same hierarchy to connect.</td>
  </tr>
  <tr>
    <td rowspan="5">Exception</td>
    <td>CRS-334</td>
    <td>Only objects can be connected</td>
  </tr>
  <tr>
    <td>CRS-335</td>
    <td>Objects with the same name cannot connect</td>
  </tr>
  <tr>
    <td>CRS-336</td>
    <td>Already connected to the object tree</td>
  </tr>
  <tr>
    <td>CRS-357</td>
    <td>Cannot Append with a different name</td>
  </tr>
  <tr>
    <td>CRS-362</td>
    <td>Objects with array elements or structures cannot be Append</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>Function OnTouch(e) {
    var child = new Array(1, 2, 3, 4, 5);
    Append(child, "TheArray");
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/system/object/methods/delete">Delete</a>, <a href="/package/system/object/methods/deletechild">DeleteChild</a> methods</td>
  </tr>
</table>



