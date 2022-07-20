---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetColFromID Method
nav_order: 37
permalink: /package/extension5/sspread/methods/getcolfromid
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Gets the column number with the specified identification string.<br><br>The <a href="/package/extension5/sspread/properties/colid">ColID</a> property can be used to set any string that identifies the column. This method can get the column number of a column that has the specified identification string set.<br><br>The identification string is not case sensitive.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetColFromID(<b>colid</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Column index</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>colid</b></td>
    <td>A string that identifies the column</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
   Col = 3;
    ColID = "address";
    print(GetColFromID("address"), "\n");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/colid">ColID</a> property</td>
  </tr>
</table>
