---
layout: default

grand_parent: XmlDOMImplementation Class
parent: Methods
has_children: false
title: XmlDOMImplementation.HasFeature Method
nav_order: 6
permalink: /package/xmlpackage/xmldomimplementation/methods/hasfeature
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Checks if it corresponds to the version specified by the <b>version</b> of the function specified by <b>feature</b>.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = domImpl.HasFeature( <b>feature, version</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">$TRUE if the specified version is supported , $FALSE if not supported</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>feature</b></td>
    <td>Function to check the version<br>Corresponds to "xml" and "dom".</td>
  </tr>
  <tr>
    <td>String <b>version</b></td>
    <td>Supported version ( Please specify in "1.0" format)</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    if (!domimpl.HasFeature("dom", "2.0")) {
        print("DOM Level2 not handled\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmldomimplementation/methods/createdocument">CreateDocument</a> method</td>
  </tr>
</table>



