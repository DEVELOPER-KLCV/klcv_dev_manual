---
layout: default

grand_parent: XmlCharacterData Class
parent: Methods
has_children: false
title: XmlCharacterData.SubstringData Method
nav_order: 5
permalink: /package/xmlpackage/xmlcharacterdata/methods/substringdata
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Extract a part of the string</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var s = cd.SubstringData( <b>offset, count</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Extracted character string</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>integer <b>offset</b></td>
    <td>Position to extract (specified by the number of characters)</td>
  </tr>
  <tr>
    <td>integer <b>count</b></td>
    <td>Extract length (specified by the number of characters)</td>
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
    text.ReplaceData(10, 3, "new text");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmltext">XmlText</a> class</td>
  </tr>
</table>



