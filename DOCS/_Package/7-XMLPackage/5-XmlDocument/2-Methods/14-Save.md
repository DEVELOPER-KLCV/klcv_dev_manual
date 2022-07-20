---
layout: default

grand_parent: XmlDocument Class
parent: Methods
has_children: false
title: XmlDocument.Save Method
nav_order: 14
permalink: /package/xmlpackage/xmldocument/methods/save
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Save the XML in a Writer object .<br><br><small><span style="color:red">Added since Ver.4.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">xmldoc.Save( <b>writer [, encoding</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>Object <b>writer</b></td>
    <td><a href="/base/readerwriter#reader-object">Writer Object</a> of save destination (object that can use WriteString method)</td>
  </tr>
  <tr>
    <td>String <b>encoding</b></td>
    <td>Encoding method<br>The character strings that can be specified are "Shift_JIS", "UTF-8", "EUC-JP", and "ISO-2022-JP". If omitted, the encoding is Shift_JIS.<br><br><small><span style="color:red">From here, added since Ver.4.2.0--></span></small>If the <a href="/package/xmlpackage/xmldomimplementation/methods/constructor#about-xml-with-a-unicode-internal-character-code">internal character code is UnicodeXML ,</a> only "UTF-8"can be specified, and if omitted, it will be"UTF-8".<br><small><span style="color:red"><--Till here</span></small></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>XML-4</td>
    <td>No valid Write object specified</td>
  </tr>
  <tr>
    <td>XML-5</td>
    <td>Does not support the WriteString (string) method</td>
  </tr>
  <tr>
    <td>XML-18</td>
    <td>Encoding is not supported</td>
  </tr>
  <tr>
    <td>XML-19</td>
    <td>Encoding failed</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var session = findHttpSession("http://host");
    var req = session.CreateRequest("path");
    xmldoc.Save(req);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



