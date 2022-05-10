---
layout: default

grand_parent: XPathResult Class
parent: Methods
has_children: false
title: XPathResult.SnapshotItem Method
nav_order: 2
permalink: /package/xpathpackage/xpathresult/methods/SnapshotItem
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var node = result.SnapshotItem( <b>index</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>integer <b>index</b></td>
    <td></td>
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
    var result = expression.Evaluate(node);
    for (var i = 0; i < result.SnapshotLength; i++) {
        print(result.SnapshotItem(i).Xml, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/xpathpackage/xpathresult/properties/snapshotlength">SnapshotLength</a> property</td>
  </tr>
</table>



