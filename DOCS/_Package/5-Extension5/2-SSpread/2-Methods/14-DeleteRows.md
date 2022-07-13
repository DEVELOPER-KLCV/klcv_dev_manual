---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.DeleteRows Method
nav_order: 14
permalink: /package/extension5/sspread/methods/deleterows
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Deletes the specified row or range.<br><br>Deleting a row does not reduce the number of rows set in the <a href="/package/extension5/sspread/properties/maxrows">MaxRows</a> property, it automatically adds a blank row at the end of the spreadsheet.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">DeleteRows(<b>row</b>, <b>numrows</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td rowspan="2">Arguments</td>
    <td><b>row</b></td>
    <td>First line number of the line range to be deleted</td>
  </tr>
  <tr>
    <td><b>numrows</b></td>
    <td>Number of lines to delete</td>
  </tr>
  <tr>
    <td rowspan="2">Exception</td>
    <td>EXT-1</td>
    <td>Invalid DeleteRows argument</td>
  </tr>
  <tr>
    <td>EXT-28</td>
    <td>An error occurred in the DeleteRows method</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    Function OnRClicked(e) {
        if (e.Col == 0 && e.Row > 0) {
            var ret = PopupMenu("行を挿入", "行を削除");
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
    <td colspan="2"><a href="/package/extension5/sspread/properties/maxrows">MaxRows</a> property<br><a href="/package/extension5/sspread/methods/deletecols">DeleteCols</a>, <a href="/package/extension5/sspread/methods/insertrows">InsertRows</a> methods</td>
  </tr>
</table>
