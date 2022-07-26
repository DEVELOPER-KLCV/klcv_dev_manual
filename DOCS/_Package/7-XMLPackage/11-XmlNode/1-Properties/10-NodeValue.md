---
layout: default

grand_parent: XmlNode Class
parent: Properties
has_children: false
title: XmlNode.NodeValue property
nav_order: 10
permalink: /package/xmlpackage/xmlnode/properties/NodeValue
---
# {{ page.title }}
The value of the node.

This property behaves differently depending on the value of the <a href="/package/xmlpackage/xmldocument">NodeType</a> property.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">NodeType property</th>
    <th class="tg-xt05">Explanation</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">ATTRIBUTE_NODE</td>
    <td class="tg-0lax">It is a string that concatenates the values of the child nodes that are the values of the attributes.<br>Changing this value will delete the child node once and create a single Text node containing the value you want to set.</td>
  </tr>
  <tr>
    <td class="tg-0lax">COMMENT_NODE</td>
    <td class="tg-0lax" rowspan="4">It will be a character string indicating the content. You can also set the value.</td>
  </tr>
  <tr>
    <td class="tg-0lax">TEXT_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">CDATA_SECTION_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">PROCESSING_INSTRUCTION_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">DOCUMENT_NODE</td>
    <td class="tg-0lax" rowspan="7">It can be written and read, but it does not affect the DOM tree and XML documents.</td>
  </tr>
  <tr>
    <td class="tg-0lax">DOCUMENT_TYPE_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">DOCUMENT_FRAGMENT_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">ELEMENT_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">ENTITY_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">ENTITY_REFERENCE_NODE</td>
  </tr>
  <tr>
    <td class="tg-0lax">NOTATION_NODE</td>
  </tr>
</tbody>
</table>

<br><small><span style="color:blue">Mobile, AI Ver is reaad-olny. Value cannot be changed.</span></small>