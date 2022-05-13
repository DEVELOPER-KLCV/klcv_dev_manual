---
layout: default

grand_parent: Object Class
parent: Methods
has_children: false
title: Object.Delete Method
nav_order: 4
permalink: /package/system/object/methods/delete
---
# {{ page.title }}


<table>
  <tr>
    <td>Explanation</td>
    <td>Disconnects the object from the object tree.<br><br>If the disconnected object is not referenced from anywhere, all connected child objects will also be disconnected in a chain.<br>Objects that are disconnected from the object tree and no longer referenced anywhere are deleted.<br>See <a href="/bizBrowserV/5/5-3/">Delete</a> for more information.<br><br><b>Array object</b><br>Calling the Delete method on an element of an array deletes only that element (and its child objects).<br> As a result, subsequent elements are carried down by the array number (index)<br><br><b>Object reuse</b><br>As a general rule, objects disconnected from the object tree cannot be reused. Please note that objects may not work properly when reconnecting and reusing the object tree. In particular, do not reuse each class that inherits the <a href="/package/standard/displayobject">DisplayObject</a> class, such as buttons and text boxes.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td>obj.Delete( )</td>
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
    //.Form1.Delete();
    //.Get("Form2.crs");
}
 </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td><a href="/package/system/object/methods/deletechild">DeleteChild</a>, <a href="/package/system/object/methods/append">Append</a> methods</td>
  </tr>
</table>



