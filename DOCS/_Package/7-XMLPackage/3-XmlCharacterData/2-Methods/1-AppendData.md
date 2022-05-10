---
layout: default

grand_parent: XmlCharacterData Class
parent: Methods
has_children: false
title: XmlCharacterData.AppendData Method
nav_order: 1
permalink: /package/xmlpackage/xmlcharacterdata/methods/appenddata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add a string</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">cd.AppendData( <b>text</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String  <b>text</b></td>
    <td>String to add</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>DOM-7</td>
    <td>NO_MODIFICATION_ALLOWED_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var text = elm.FirstChild;
    text.AppendData("abcdefg");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmltext">XmlText</a> class</td>
  </tr>
</table>



