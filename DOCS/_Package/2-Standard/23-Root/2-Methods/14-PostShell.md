---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.PostShellEvent Property
nav_order: 14
permalink: /package/standard/root/methods/postshellevent
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">var ret = //.PostShellEvent( <b>str</b> )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2"></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>str</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>PKG-2</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-3</td>
    <td></td>
  </tr>
  <tr>
    <td>PKG-4</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
<Biz/Browser>

//.ShellId = "Biz3";
var retval = //.PostShellEvent("from Biz/Browser");
print(retval, "\n");

BizEvent events can be received in a script in HTML as follows:

&lt;Internet Explorer&gt;

&lt;OBJECT ID="BizIEServer" CLASSID="CLSID:16137039-D27E-4BB8-9B02-B20C06B8DCBF"&gt;
&lt;SCRIPT LANGUAGE="JavaScript"&gt;
BizIEServer.ServerId = "Biz3";
&lt;/SCRIPT&gt;
&lt;SCRIPT LANGUAGE="JavaScript" FOR="BizIEServer" EVENT="BizEvent(value)"&gt;
    alert(value);
    BizIEServer.UserValue = "from JavaScript";
&lt;/SCRIPT&gt;
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/shellid">ShellId</a> method</td>
  </tr>
</table>



