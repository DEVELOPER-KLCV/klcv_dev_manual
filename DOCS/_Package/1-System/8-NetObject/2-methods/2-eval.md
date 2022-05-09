---
layout: default

grand_parent: NetObject Class
parent: Methods
has_children: false
title: NetObject.Eval Method
nav_order: 2
permalink: /package/system/netobject/methods/eval
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Run the CRS script. <br>Executing a script with the Eval method works the same as executing a Function from the caller. The CRS script to be executed can be given as a string by the <b>crs</b> argument, and the return value can be returned by the return statement, which is the return value of the Eval method.<br><small>Added since Version 4.2.0 <br>Not supported in Mobile</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">obj.Eval( <b>crs</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Depends on the script's return statement</td>
  </tr>  
  <tr>
    <td>Argument</td>
    <td>String <b>crs</b></td>
    <td>Specify the CRS script as a string.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>var t = Eval("return new " + str(type) + ";");
Append(t, "data");</pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



