---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.Truncate Method
nav_order: 11
permalink: /package/system/object/methods/truncate
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td>Deletes all the elements of the arrayed object.<br><br>This method only attaches array objects. This method has no effect on non-arrayed objects.<br><br>It works faster than repeating the <a href="/package/system/object/methods/delete">Delete</a> method for individual array elements.<br>Unlike calling the <a href="/package/system/object/methods/delete">Delete</a> method on an array object, the definition is not deleted, so it it possible to recreate the array element with the <a href="/package/system/object/methods/insert">Insert</a> method later.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.Truncate( )</td>
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
Record arrayRec[5] {
    Number numItem;
    String strItem;
}
arrayRec.Truncate(); 
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td><a href="/package/system/object/methods/insert">Insert</a> method</td>
  </tr>
</table>



