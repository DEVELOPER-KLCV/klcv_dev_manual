---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.RemBookmark Property
nav_order: 17
permalink: /package/standard/root/methods/rembookmark
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Delete the bookmark entry.<br><br>Specify a URL that is already registered in the bookmark and delete the bookmark.<br><br>When running a test from Biz / Designer, the edited bookmarks are not saved and will be restored at the end of the test run.<br><small><span style="color:red">Added since Ver.4.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.RemBookmark( [ <b>URL</b> ] )<br><small><span style="color:green">Arguments can now be omitted since Version 5.0.0</span></small></td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>String <b>URL</b></td>
    <td>URL of the bookmark to be deleted<br><br><small><span style="color:green">The following specifications have been added since Version 5.0.0</span></small><br>If omitted, or if an empty string is specified, all bookmarks will be deleted.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.RemBookmark("http://server/app/menu.crs");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/setbookmark">SetBookmark</a>, <a href="/package/standard/root/methods/getbookmark">GetBookmark</a> methods</td>
  </tr>
</table>



