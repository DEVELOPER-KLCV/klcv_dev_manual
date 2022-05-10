---
layout: default

grand_parent: XPathEvaluator Class
parent: Methods
has_children: false
title: XPathEvaluator.CreateNSResolver Method
nav_order: 2
permalink: /package/xpathpackage/xpathevaluator/methods/CreateNSResolver
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var resolver = XPathEvaluator.CreateNSResolver( <b>node</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XmlNode <b>node</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>    	
    var xpath = "/svg.g[@id=\"layer\"]";
    var svgdoc = dom.DocumentElement;
    var resolver = XPathEvaluator.CreateNSResolver(dom);
    var expression = XPathEvaluator.CreateExpression(xpath, resolver);
    var result = expression.Evaluate(svgdoc);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



