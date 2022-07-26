---
layout: default

grand_parent: XmlText Class
parent: Methods
has_children: false
title: XmlText.SplitText Method
nav_order: 1
permalink: /package/xmlpackage/xmltext/methods/splittext
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Splits the Text node at the specified position into two Text nodes.<br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var text2 = text.SplitText( <b>offset</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlText object containing the second half of the split text</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>offset</b></td>
    <td>Split position (specified by the number of characters)</td>
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
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var text1 = xmldoc.DocumentElement.FirstChild;
    var text2 = text1.SplitText(20);
    print(text1.Data, "\n");
    print(text2.Data, "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



