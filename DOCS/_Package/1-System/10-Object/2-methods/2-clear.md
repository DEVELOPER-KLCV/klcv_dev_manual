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
    <td>Initializes the object's default properties.<br><br> <b>Initialization</b> <br> Initialization is done according to the data type of the default property ( <a href="/package/system/object/properties/valuetype">ValueType</a> of the object). (It does not return to the initial value set when the object was created).<br>For example, a String object is initialized to an empty string, and a Number object is initialized to 0.<br><br> The Clear method differs from assigning an initial value to a default property in that it can be initialized without being aware of the details of the object to be operated.<br>Even if the operation target has different values ​​to be initialized such as Number object and String object , it can be safely initialized by the same procedure by the Clear method. <br><br> <b>Default property</b><br> The default property is the Value property in many classes, but some classes have other properties as default properties.<br>Also, some classes do not have default properties. The Clear method has no effect on classes that do not have default properties.<br>See the documentation for each class for default properties.<br><br> <b>Array object</b><br>Executing the Clear method on an array object does not affect each element object. The Clear method need to be executed individually for the array element object.</td>
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



