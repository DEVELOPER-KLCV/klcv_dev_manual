---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.Insert Method
nav_order: 10
permalink: /package/system/object/methods/insert
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add an element to the arrayed object.<br><br>This method is attached only to array objects and array elements. This method has no effect on non-arrayed objects.<br><br>Running on an array object inserts a new element at the end of the array.<br>When executed on an array element, a new element is inserted at the previous position.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.Insert( [ <b>count</b> ] )<br>obj[ <b>index</b> ].Insert( [ <b>count</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td>None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>count</b></td>
    <td>Specifies the number of elements to insert. If omitted, one item will be inserted.</td>
  </tr>
  <tr>
    <td>integer <b>index</b></td>
    <td>Specify the insertion position with a subscript. The element at the specified position must exist.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td><code><pre>
/* Usage example for array objects */
Record arrayRec[] {
    Number numItem;
    String strItem;
}
arrayRec.Insert(10);
 
/* Usage example for array elements */
Record arrayRec[5] {
    Number numItem;
    String strItem;
}
arrayRec[1].Insert(2);
 
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td><a href="/package/system/object/methods/truncate">Truncate</a> method</td>
  </tr>
</table>



