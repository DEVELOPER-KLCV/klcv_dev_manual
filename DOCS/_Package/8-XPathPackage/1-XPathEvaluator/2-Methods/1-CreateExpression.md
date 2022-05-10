---
layout: default

grand_parent: XPathEvaluator Class
parent: Methods
has_children: false
title: XPathEvaluator.CreateExpression Method
nav_order: 1
permalink: /package/xpathpackage/xpathevaluator/methods/createexpression
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var expression = XPathEvaluator.CreateExpression( <b>xpath, resolver</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>xpath</b></td>
    <td></td>
  </tr>
  <tr>
    <td>XPathNSResolver <b>resolver</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>XPath-51</td>
    <td>EXPRESSION_ERR</td>
  </tr>
  <tr>
    <td>XPath-52</td>
    <td>TYPE_ERR</td>
  </tr>
  <tr>
    <td>DOM-14</td>
    <td>NAMESPACE_ERR</td>
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



