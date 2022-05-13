---
layout: default

grand_parent: Exception Class
parent: Methods
has_children: false
title: Exception constructor
nav_order: 1
permalink: /package/system/exception/methods/constructor
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize the Exception object.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ex = new Exception ( <b>method , code , message</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Exception object</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>String <b>method</b></td>
    <td>Specifies the value of the Method property.</td>
  </tr>
  <tr>
    <td>integer <b>code</b> </td>
    <td>Specifies the value of the Code property</td>
  </tr>
 <tr>
    <td>String  <b>message</b> </td>
    <td>Specifies the value of the Message property</td>
  </tr> 
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>if (data == 0) {
    throw new Exception ("APP1", 1, "data is 0 ") ;
}</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



