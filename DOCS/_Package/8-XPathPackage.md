---
layout: default
has_children: true

title: 8. XPath Package
nav_order: 8
permalink: /package/xpathpackage
has_toc: false
---

# {{ page.title }}

It is a package for handling XPath used in XML.

The XPath package is a subset of the DOM (Document Object Model) Level 3 XPath Version 1.0 defined by the W3C (World Wide Web Consortium), excluding some features.

<u><b>Class</b></u>

<table>
    <tr>
        <td rowspan="2">Name</td>
        <td rowspan="2">Explanation</td>
        <td>Version</td>
    </tr>
    <tr>
        <td>PC</td>
        <td>Mobile</td>
        <td>AI</td>
    </tr>
    <tr>
        <td><a href="/package/xpathpackage/xpathevaluator">XPathEvaluator</a></td>
        <td>A class that creates each XPath object</td>
        <td>4.0.0</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td><a href="/package/xpathpackage/XPathException">XPathException</a></td>
        <td>Exceptions that occur with XPath packages</td>
        <td>4.0.0</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td><a href="/package/xpathpackage/XPathExpression">XPathExpression</a></td>
        <td>Perform XPath parsing</td>
        <td>4.0.0</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td><a href="/package/xpathpackage/XPathNSResolver">XPathNSResolver</a></td>
        <td>A class for resolving namespace prefixes in XPath evaluation</td>
        <td>4.0.0</td>
        <td>-</td>
        <td>-</td>
    </tr>
    <tr>
        <td><a href="/package/xpathpackage/XPathResult">XPathResult</a></td>
        <td>Holds XPath results</td>
        <td>4.0.0</td>
        <td>-</td>
        <td>-</td>
    </tr>
</table>

**About W3C DOM Level3 XPath**

Document Object Model (DOM) Level 3 XPath Specification Version 1.0 published by W3C is a Candidate Recommendation at the time of release of Biz / Browser ver4.0.0 (August 2003).
W3C will continue to formulate specifications in the future, but it is estimated that the functions built into Biz / Browser ver3.0 will not undergo major changes because the specifications have already been mostly finalized. Will be done.

**Unsupported object**

The following objects included in W3C DOM Level3 XPath are not supported by Biz / Browser and cannot be used.

    XPathNamespace interface

**About XPath syntax (Expression) compatibility**

The available XPath syntax conforms to the W3C-recommended XML Path Language (XPath) Version 1.0 W3C Recommendation 16 November 1999 document, with the following exceptions:

1. All numbers are represented by signed integers.

1. Namespace resolution does not consider relative paths.

1. Refers only to the default namespaces that XPathResolver can resolve in namespace resolution. This is usually the default namespace defined in the DocumentElement. It is not possible to handle the default namespace depending on the context node.

1. Operations that utilize the XPathNamespace interface are replaced by attribute operations. Also, when the XPathNamespace object is selected as a result, it is replaced by the XmlAttr object.

1. The XPath evaluation result is always ORDERED_NODE_SNAPSHOT_TYPE. If you specify other types such as numbers, strings, iterators, etc., the result converted from ORDERD_NODE_SNAPSHOT is returned.

In Biz / Browser, it was possible to easily search for Node using a subset of XPath syntax with the XmlNode.SelectNodes and XmlNode.SelectSingleNode methods from ver3.0, but the XPath package extended from ver4.0.0 Not compatible with XPath syntax. Please be aware of the difference in behavior when using it.

**Typical usage**

The XPath package creates an [XPathNSResolver](/package/xpathpackage/xpathnsresolver) object and an [XPathExpression](/package/xpathpackage/xpathexpression) object by a static method of the [XPathEvaluator](/package/xpathpackage/xpathevaluator) class, evaluates the XPath syntax by the [XPathExpression.Evaluate](/package/xpathpackage/xpathexpression/methods/evaluate) method, and receives the result in the [XPathResult](/package/xpathpackage/xpathresult) object.

```
/* Download the XML document */
var session = getHttpSession();
var response = session.Get("data.xml");
 
/* Create a DOM tree */
var domImpl = new XmlDOMImplementation;
var dom = domImpl.Load(response);
 
/* Prepare for XPath search */
var resolver = XPathEvaluator.CreateNSResolver(dom);
var expression = XPathEvaluator.CreateExpression("//x", resolver);
 
/* Perform a search */
var result = expression.Evaluate(dom.documentElement, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE);
 
/* Check the search results */
var len = result.SnapshotLength;
for (var i = 0; i < len; i++) {
    var node = result.SnapshotItem(i);
    print("No " + str(i + 1) + ": " + node.xml, "\n");
}
 
----- Execution result -----
No 1: <x name="x1">
No 2: <x name="x2">
No 3: <x name="x3">
No 4: <x name="x4">
No 5: <x name="x5">
```

### XPath syntax example

#### child :: para
##### para
    Select the para node from the children of the context node.

#### child :: *
##### *
    Select all child nodes of the context node.

#### child :: text ()
##### text ()
    Select all non-empty text nodes among the child nodes of the context node.

#### child :: node ()
##### node ()
    Select all child nodes of the context node.

#### attribute :: name
##### @name
    Select the name attribute of the context node.

#### attribute :: *
##### @ *
    Select all attributes of the context node.

#### descendant :: para
    Select all para nodes from the descendants of the context node.

#### ancestor :: div
    Select all div nodes from the ancestors of the context node.

#### ancestor-or-self :: div
    Select all div nodes from the context node and its ancestors.

#### descendant-or-self :: para
    Select all para nodes from the context node and its descendants.

#### self :: para
    If the context node is para Select the context node.

#### child :: chapter / descendant :: para
##### chapter // para
    Select all para nodes from the descendants of the chapter node, which is a child of the context node.

#### child :: * / child :: para
##### * / para
    Select all para nodes from the grandchild nodes of the context node.

#### / 
    If specified at the beginning, selects the document root.

#### / descendant :: para
    Select all para nodes in the document.


#### / descendant :: olist / child :: item
    Select all item nodes from the children of the olist node in the document.

#### child :: para [position () = 1]
##### para [1]
    Select the first para node from the child nodes of the context node.

#### child :: para [position () = last ()]
##### para [last ()]
    Select the last para node from the child nodes of the context node.

#### child :: para [position () = last ()-1]
##### para [last ()-1]
    Select the penultimate para node from the child nodes of the context node.

#### child :: para [position ()> 1]
    Select all the second and subsequent para nodes from the child nodes of the context node.

#### following-sibling :: chapter [position () = 1]
    Select the first chapter node from the siblings that follow the context node.

#### preceding-sibling :: chapter [position () = 1]
    Select the first chapter node from the siblings that precede the context node.

#### / descendant :: figure [position () = 42]
    Select the 42nd node from all figure nodes in the document.

#### / child :: doc / child :: chapter [position () = 5] / child :: section [position () = 2]
##### / doc / chapter [5] / section [2]
    Select the second section node of the fifth chapter from the child of the document element doc.

#### child :: para [attribute :: type = "warning"]
##### para [@type = "warning"]
    Select all para nodes with "warning" in the type attribute from the children of the context node.

#### child :: para [attribute :: type = "warning"] [position () = 5]
##### para [@type ='warning'] [5]
    Select the 5th para node with "warning" in the type attribute from the children of the context node.

#### child :: para [position () = 5] [attribute :: type = "warning"]
##### para [5] [@type = "warning"]
    If the type attribute of the 5th para node from the child of the context node has "warning", select it.

#### child :: chapter [child :: title = "Introduction"]
##### chapter [title = "Introduction"]
    Among the child node chapters of the context node, select the node with "Introduction" in the title.

#### child :: chapter [child :: title]
##### chapter [title]
    Among the child node chapters of the context node, select the node that has the title node as a child.

#### child :: * [self :: chapter or self :: appendix]
    Select all chapter or appendix nodes from all child nodes of the context node.

#### child :: * [self :: chapter or self :: appendix] [position () = last ()]
    Of all the child nodes of the context node, select the last node that has a chapter node or an appendix node.

#### / descendant-or-self :: node () / child :: chapter [position () = 2]
##### // chapter [2]
    Select all the second chapter nodes of all the nodes in the document.
 

