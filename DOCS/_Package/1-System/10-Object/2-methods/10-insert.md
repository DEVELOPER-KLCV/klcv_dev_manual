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
    <td></td>
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
    <td></td>
  </tr>
  <tr>
    <td>integer <b>index</b></td>
    <td></td>
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



