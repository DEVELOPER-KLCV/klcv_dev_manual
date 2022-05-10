---
layout: default

grand_parent: XPathExpression Class
parent: Methods
has_children: false
title: XPathExpression.Evaluate Method
nav_order: 1
permalink: /package/xpathpackage/xpathexpression/methods/evaluate
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var result = expression.Evaluate( <b>node [, type [, result ] ]</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>XmlNode <b>node</b></td>
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
    var resolver = XPathEvaluator.CreateNSResolver(node);
    var expression = XPathEvaluator.CreateExpression(xpath, resolver);
    var result = expression.Evaluate(node);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
</table>



