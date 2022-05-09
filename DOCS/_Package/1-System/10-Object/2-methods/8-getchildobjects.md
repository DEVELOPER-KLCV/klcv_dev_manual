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
    <td>Gets all child objects connected to the object. <br><small>Added ssince ver.3.0.0</small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.GetChildObjects( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td><a href="/package/system/array">Array</a> object containing all child objects.<br><br>Returns an Array object that contains a reference for the child object. The elements of the Array object are stored as an associative array with the name of the child object as the key. To access the stored child objects, either specify the name as a string in the form of <br><code><pre>childArray [" object name "]</pre></code><br> or access them sequentially in a for in loop like <br><code><pre>for (var i in childArray) {
       print (childArray [i] .value, "\ n");
       :
}</pre></code><br>Keep in mind that access by name is case sensitive.<br><br>The GetChildObjects method does not get the array elements of the arrayed child objects. If you need access to an array element, do the following:<br><code><pre>
var childArray = GetChildObjects ();
var obj = childArray ["item"] [index];</pre></code>
</td>
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



