---
layout: default

grand_parent: XPathResult Class
parent: Methods
has_children: false
title: XPathResult.IterateNext Method
nav_order: 1
permalink: /package/xpathpackage/xpathresult/methods/iteratenext
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = result.IterateNext( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td>XPath-52</td>
    <td>TYPE_ERR</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    var resolver = XPathEvaluator.CreateNSResolver(node);
    var expression = XPathEvaluator.CreateExpression(xpath, resolver);
    var result = expression.Evaluate(node, XPathResult.ORDERED_NODE_ITERATOR_TYPE);
    while ((var node = result.IterateNext()) != null){
        print(node.Xml, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xpathpackage/xpathresult/properties/invaliditeratorstate">invalidIteratorState</a> property</td>
  </tr>
</table>



