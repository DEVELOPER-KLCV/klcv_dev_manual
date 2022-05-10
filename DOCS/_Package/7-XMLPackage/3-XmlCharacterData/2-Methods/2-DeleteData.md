---
layout: default

grand_parent: XmlCharacterData Class
parent: Methods
has_children: false
title: XmlCharacterData.DeleteData Method
nav_order: 2
permalink: /package/xmlpackage/xmlcharacterdata/methods/deletedata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete the string</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">cd.DeleteData( <b>offset, count</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>offset</b></td>
    <td>Position to delete (specified by the number of characters)</td>
  </tr>
  <tr>
    <td>integer <b>count</b></td>
    <td>Length to delete (specified by the number of characters)</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>DOM-1</td>
    <td>INDEX_SIZE_ERR</td>
  </tr>
  <tr>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var text = elm.FirstChild;
    text.DeleteData(10, 3); 
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmltext">XmlText</a> class</td>
  </tr>
</table>



