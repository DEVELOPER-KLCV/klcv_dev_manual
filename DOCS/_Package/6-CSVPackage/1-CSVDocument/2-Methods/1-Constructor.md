---
layout: default

grand_parent: CSVDocument Class
parent: Methods
has_children: false
title: CSVDocument Constructor
nav_order: 1
permalink: /package/csvpackage/csvdocument/methods/constructor
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Initialize CSVDocument. <br><br><small><span style="color:red">Added since Ver.4.2.0 from here--></span></small>
    <br>If specified <b><i>enc</i></b> in CSVDocument, the internal character code will be in Unicode. If ommitted, the multi-byte character code (Shift-JIS if in Japanese environment) depends on the platform language.<br><small><span style="color:red"><--till here</span></small><br><br><small><span style="color:red">Added since Ver.5.3.0 from here--></span></small><br>When specifying CSVDocument:UString and the data-type is specified as UString, it is the same as specifying Constructor in CSVDocument.Unicode.
    <br><small><span style="color:red"><--till here</span></small><br><br><small><span style="color:green">Since AI Ver.1.0.1 the internal character code will always be in UTF-8.</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var csvdoc = new CSVDocument( [ <b><i>enc</i></b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">CSVDocument object</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b><i>enc</i></b></td>
    <td>Specify internal character code. <br>Currently, character code that can be specified is only CSVDocument.Unicode. <br>If omitted it will be in multi-byte code(Shift-JIS in case of Japanese environment).<br><br><small><span style="color:red">Added since Ver.4.2.0</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small><br><small><span style="color:grey">More obsolute than AI Ver.1.0.1. Internal character code will always be UTF-8. </span></small>
    </td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var csvdoc = new CSVDocument(CSVDocument.Unicode);
    var res = session.Get("/test/sample.csv");
    csvdoc.Load(res);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>


### <i>About CSVDocument which internal character code is Unicode(PC ver, Mobile ver)</i>

If CSVDocument.Unicode is specified as an argument, the internal character code is treated as Unicode.
<br>If want to use Unicode-specific characters or characters that are not in the platform character code (Shift-JIS in Japanese) for the data to be handled, set the internal character code to Unicode.

If the internal character code is set as Unicode, you need to save CSV file in Unicode (UTF-16) format using <a href="/package/csvpackage/csvdocument/methods/get">Get</a> method, <a href="/package/csvpackage/csvdocument/methods/load">Load</a> method. If file is saved in Multi-byte code(Shift-JIS or UTF-8 etc.), the CSV file cannot be read. If <a href="/package/csvpackage/csvdocument/methods/save">Save</a> method is used, the format will be in Unicode (UTF-16).

### <br><i>About CSVDocument character code in Biz/Browser AI (Android ver)</i>

<br>From Biz / Browser AI 1.0.1, the internal character code of CSV Document is always UTF-8. Therefore, the CSV file loaded by the 
<a href="/package/csvpackage/csvdocument/methods/get">Get</a> method and <a href="/package/csvpackage/csvdocument/methods/load">Load</a> method must be saved in UTF-8 format. CSV files saved with other character codes (Shift-JIS, Unicode (UTF-16), etc.) cannot be read. Saving by the <a href="/package/csvpackage/csvdocument/methods/save">Save</a> method is also in UTF-8 format.




