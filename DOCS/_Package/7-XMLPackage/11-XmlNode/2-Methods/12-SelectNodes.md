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
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var list = node.SelectNodes( <b>xpath</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>xpath</b></td>
    <td></td>
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



