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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = domImpl.HasFeature( <b>feature, version</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>feature</b></td>
    <td></td>
  </tr>
  <tr>
    <td>String <b>version</b></td>
    <td></td>
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



