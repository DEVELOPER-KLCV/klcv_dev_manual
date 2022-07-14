---
layout: default

grand_parent: SSpread Class
parent: Methods
has_children: false
title: SSpread.GetSelection Method
nav_order: 48
permalink: /package/extension5/sspread/methods/getselection
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Returns one of the selected cell blocks on the spreadsheet.<br><br>Gets the selected cell blocks if the user is allowed to select multiple cell blocks (if the <a href="/package/extension5/sspread/properties/allowmultiblocks">AllowMultiBlocks</a> property is $TRUE).<br>The index of the cell block is specified in the argument index. Cell block indexes are assigned serial numbers starting from 0, starting with the largest block.<br><br>The total number of selected cell blocks can be obtained with the <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> property.<br><br> Use the <a href="/package/extension5/sspread/methods/addselection">AddSelection</a> method to add a selected cell block.</td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">GetSelection(<b>index</b>)</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Record object with the following child objects<br><style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-ihln{font-style:italic;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-23hc{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-z50u{background-color:#D9D9D9;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:center;
  vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23hc">Type</th>
    <th class="tg-z50u">Name</th>
    <th class="tg-23hc">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Col</td>
    <td class="tg-0lax">Leftmost column number of the selected cell block</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Row</td>
    <td class="tg-0lax">Row number at the top of the selected cell block</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Col2</td>
    <td class="tg-0lax">Rightmost column number of the selected cell block</td>
  </tr>
  <tr>
    <td class="tg-0lax">Number</td>
    <td class="tg-ihln">Row2</td>
    <td class="tg-0lax">Row number at the bottom of the selected cell block</td>
  </tr>
</tbody>
</table></td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td><b>index</b></td>
    <td>Cell block index number</td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    AllowMultiBlocks = $TRUE;
    AddSelection(2, 2, 4, 3);
    AddSelection(1, 5, 5, 5);
    AddSelection(2, 7, 4, 7);
    for (var n = 0; n < SelectionCount; n++) {
        var sel = GetSelection(n);
        print(sel.Col, sel.Row, sel.Col2, sel.Row2, "\n");
    }
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/extension5/sspread/properties/allowmultiblocks">AllowMultiBlocks</a>, <a href="/package/extension5/sspread/properties/selectioncount">SelectionCount</a> property<br><a href="/package/extension5/sspread/methods/addselection">AddSelection</a> method</td>
  </tr>
</table>
