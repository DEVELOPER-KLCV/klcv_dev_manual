---
layout: default

grand_parent: XmlCharacterData Class
parent: Methods
has_children: false
title: XmlCharacterData.InsertData Method
nav_order: 3
permalink: /package/xmlpackage/xmlcharacterdata/methods/insertdata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Insert a string</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">cd.InsertData( <b>offset, text</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>offset</b></td>
    <td>Position to add (specified by the number of characters)</td>
  </tr>
  <tr>
    <td>String <b>text</b></td>
    <td>String to add</td>
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
    text.InsertData(10, "abcdefg");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmltext">XmlText</a> class</td>
  </tr>
</table>



