---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.IsSupported Method
nav_order: 6
permalink: /package/xmlpackage/xmlnode/methods/IsSupported
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Check the implementation of the feature.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = node.IsSupported( <b>feature, version</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$TRUE if the version specified in version of the feature specified is supported,$FALSE otherwise</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>feature</b></td>
    <td>Function to check<br>Specify the function with the following character string.<br>"Core"<br>"XML"<br>"HTML"<br>"Views"<br>"CSS"</td>
  </tr>
  <tr>
    <td>String <b>version</b></td>
    <td>Version to be checked<br>The version is a string like this:<br>"1.0"<br>"2.0"</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    if (node.IsSupported("XML", "2.0")) {
        return;
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



