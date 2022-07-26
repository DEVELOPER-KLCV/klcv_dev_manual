---
layout: default

grand_parent: XmlNode Class
parent: Methods
has_children: false
title: XmlNode.SelectNodes Method
nav_order: 12
permalink: /package/xmlpackage/xmlnode/methods/selectnodes
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Searches for nodes that match the conditions specified in XPath .</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var list = node.SelectNodes( <b>xpath</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">XmlNodeList object containing all the nodes that match the criteria</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>xpath</b></td>
    <td>Specify the search conditions in XPath format.<br>The following elements can be specified for XPath.<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">// name</th>
    <th class="tg-0lax">Select the name element from the current child and descendant elements .</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">../name</td>
    <td class="tg-0lax">Select the element with name from the children of the current parent element .</td>
  </tr>
  <tr>
    <td class="tg-0lax">name/*</td>
    <td class="tg-0lax">Selects all child elements of the name element from the current child elements .</td>
  </tr>
  <tr>
    <td class="tg-0lax">name@id</td>
    <td class="tg-0lax">Select the id attribute of the name element from the current child elements .<br><small><span style="color:blue">Not supported in Mobile</span></small></td>
  </tr>
  <tr>
    <td class="tg-0lax">name[.="data"]</td>
    <td class="tg-0lax">Select the name element with the value data from the current child elements .</td>
  </tr>
  <tr>
    <td class="tg-0lax">name [@id="data"]</td>
    <td class="tg-0lax">Selects the name element with an id attribute of data from the current child elements .</td>
  </tr>
  <tr>
    <td class="tg-0lax">name [2]</td>
    <td class="tg-0lax">Select the third name element from the current child elements .<br><small><span style="color:green">Index starts from 1 in AI Ver.</span></small></td>
  </tr>
</tbody>
</table>
<br><small><span style="color:red">Added since Ver.4.1.2 from here--></span></small><br>Added support for searches that specify NodeType such as #text.<br><small><span style="color:red"><--Up to here</span></small></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    /*
    SelectNodes("//CODE");
        Finds the CODE element in the entire DOM tree.
    SelectNodes("/DATA/USER_REC/USERNAME[.="tanaka"]");
        Finds the element with the value tanaka in / DATA / USER_REC / USERNAME.
    SelectNodes("//CODE/USER_REC[0]");
        Search the entire DOM tree for the CODE element and select the beginning of its child USER_REC.
    */
    
    var domimpl = new XmlDOMImplementation;
    var res = session.Get("/test/sample.xml");
    var xmldoc = domimpl.Load(res);
    var list = xmldoc.DocumentElement.SelectNodes("//CODE");
    for (var n in list) {
        print(list.Item(n).NodeName, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xmlpackage/xmlnodelist">XmlNodeList</a> class<br>,<a href="/package/xmlpackage/xmlnode/methods/selectsinglenode">SelectSingleNode</a> method</td>
  </tr>
</table>



