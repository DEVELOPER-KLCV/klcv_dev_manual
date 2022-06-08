---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.GetBookmark Property
nav_order: 5
permalink: /package/standard/root/methods/getbookmark
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Get a list of bookmarks.<br><br>Bookmark is a list of connection destination URLs saved by Biz / Browser and is automatically registered at login. The bookmark is retained even if you quit Biz / Browser, and you can use it the same way the next time you start it. The bookmark list is displayed on the standard login screen of Biz / Browser, and you can select the URL of the login destination. You can add a title string to the bookmark. Edit bookmarks with the SetBookmark and RemBookmark methods. <br><br><small><span style="color:red">Added since Ver.4.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small>
  <tr>
    <td>Call format</td>
    <td colspan="2">var list = //.GetBookmark( )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns an array of Record objects with the following child objects: <br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-t0bo{background-color:#c0c0c0;border-color:inherit;color:#000000;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-t0bo">Type</th>
    <th class="tg-t0bo">Name</th>
    <th class="tg-t0bo">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">String</td>
    <td class="tg-0pky">url</td>
    <td class="tg-0pky">Bookmark URL</td>
  </tr>
  <tr>
    <td class="tg-0pky">String</td>
    <td class="tg-0pky">title</td>
    <td class="tg-0pky">Bookmark title</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    var list = //.GetBookmark();
    for (var n = 0; n < list.length; n++) {
        print(list[n].url, list[n].title, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/methods/setbookmark">SetBookmark</a>, <a href="/package/standard/root/methods/rembookmark">RemBookmark</a> method</td>
  </tr>
</table>



