---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetBookmark Property
nav_order: 20
permalink: /package/standard/root/methods/setbookmark
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Add or change bookmark entries.<br><br>If you specify a new URL, it will be added to the end of the bookmark list.<br>If you specify the same URL as the one already registered, the title of the bookmark will be replaced.<br><br>When running a test from Biz / Designer, the edited bookmarks are not saved and will be restored at the end of the test run.<br><small><span style="color:red">Added since Ver.4.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">///.SetBookmark( <b>URL</b> [, <b>title</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td>String <b>URL</b></td>
    <td>URL of bookmark to add or change<br>Only character strings that can be recognized as URLs can be registered correctly.</td>
  </tr>
  <tr>
    <td>String <b>title</b></td>
    <td>Bookmark title<br>If omitted, the title will be blank.</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    //.SetBookmark("http://server/app/menu.crs", "業務メニュー");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/rembookmark">RemBookmark</a>, <a href="/package/standard/root/methods/getbookmark">GetBookmark</a> method</td>
  </tr>
</table>



