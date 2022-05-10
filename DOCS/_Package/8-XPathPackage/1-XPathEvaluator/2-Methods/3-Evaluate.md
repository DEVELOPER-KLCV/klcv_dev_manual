---
layout: default

grand_parent: XPathEvaluator Class
parent: Methods
has_children: false
title: XPathEvaluator.Evaluate Method
nav_order: 3
permalink: /package/xpathpackage/xpathevaluator/methods/Evaluate
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var result = XPathEvaluator.Evaluate( <b>xpath, node, resolver [, type [, result ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="5">Arguments</td>
    <td>String <b>xpath</b></td>
    <td></td>
  </tr>
  <tr>
    <td>XmlNode <b>node</b></td>
    <td></td>
  </tr>
  <tr>
    <td>XPathNSResolver <b>resolver</b></td>
    <td></td>
  </tr>
  <tr>
    <td>integer <b>type</b></td>
    <td></td>
  </tr>
  <tr>
    <td>XPathResult <b>result</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="4">Exception</td>
    <td>XPath-51</td>
    <td>EXPRESSION_ERR</td>
  </tr>
  <tr>
    <td>XPath-52</td>
    <td>TYPE_ERR</td>
  </tr>
  <tr>
    <td>DOM-4</td>
    <td>WRONG_DOCUMENT_ERR</td>
  </tr>
  <tr>
    <td>DOM-14</td>
    <td>NAMESPACE_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>    	
    var xpath = "/svg.g[@id=\"layer\"]";
    var svgdoc = dom.documentElement;
    var resolver = XPathEvaluator.CreateNSResolver(dom);
    var result = XPathEvaluator.Evaluate(xpath, svgdoc, resolver);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



