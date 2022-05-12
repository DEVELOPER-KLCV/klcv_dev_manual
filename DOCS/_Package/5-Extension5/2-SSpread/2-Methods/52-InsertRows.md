---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.InsertRows Method
nav_order: 52
permalink: /package/extension5/sspread/methods/insertrows
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">InsertRows(<b>row</b>, <b>numrows</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>row</b></td>
    <td></td>
  </tr>
  <tr>
    <td><b>numrows</b></td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td></td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td></td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function OnRClicked(e) {
        if (e.Col == 0 && e.Row > 0) {
            var ret = PopupMenu("Add row", "Delete row");
            switch (ret) {
            case 1:
                InsertRows(e.Row, 1);
                break;
            case 2:
                DeleteRows(e.Row, 1);
                break;
            }
        }
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/maxrows">MaxRows</a> property<br><a href="/package/extension5/sspread/methods/deleterows">DeleteRows</a>, <a href="/package/extension5/sspread/methods/insertcols">InsertCols</a> methods</td>
  </tr>
</table>
