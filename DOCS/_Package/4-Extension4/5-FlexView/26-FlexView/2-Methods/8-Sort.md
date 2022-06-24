---
layout: default

grand_parent: FlexView Class
parent: Methods
has_children: false
title: FlexView.Sort Method
nav_order: 8
permalink: /package/extension4/flexview/flexview/methods/sort
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2">Sorts the rows by the column at the specified position<br><small><span style="color:red">Added since Ver.4.1.0</span></small></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">FlexView1.Sort ( <b><i>col</i></b> [, <b><i>arr</i></b> [, <b><i>prop</i></b> ]])</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">Returns a reference to the <a href="/package/extension4/flexview/flexrow">FlexRow</a> object that points to the first row inserted.</td>
  </tr>  
  <tr>
    <td rowspan="3">Arguments</td>
    <td>integer <b><i>col</i></b></td>
    <td>Specifies the number of columns to sort</td>
  </tr>
  <tr>
    <td>string <b><i>arr</i></b></td>
    <td>Specify the sort direction.<br>
   <style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-34fe{background-color:#c0c0c0;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-llyw{background-color:#c0c0c0;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
 <table class="tg">
 <thead>
  <tr>
    <th class="tg-34fe">Value</th>
    <th class="tg-llyw">Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
    <td class="tg-c3ow">"a"</td>
    <td class="tg-0pky">Sort in ascending order</td>
  </tr>
  <tr>
    <td class="tg-c3ow">"d"</td>
    <td class="tg-0pky">Sort in descending order</td>
  </tr>
  <tr>
    <td class="tg-c3ow">"aq"</td>
    <td class="tg-0pky">Sort in ascending order with quicksort</td>
  </tr>
  <tr>
    <td class="tg-c3ow">"dq"</td>
    <td class="tg-0pky">Sort in descending order with quicksort</td>
  </tr>
 </tbody>
 </table>
    <br>If omitted or other than the above, sort in ascending order.</td>
  </tr>
    <tr>
    <td>string <b><i>prop</i></b></td>
    <td>Specify the property to be used as the sort key as a string. If omitted, the operation is the same as when "value" is specified.</td>
  </tr>
  <tr>
    <td rowspan="3">Exception</td>
    <td>EXT-6</td>
    <td>FlexRecord not found</td>
  </tr>
    <tr>
    <td>EXT-14</td>
    <td>Column not found</td>
  </tr>
      <tr>
    <td>EXT-17</td>
    <td>Property not found</td>
  </tr>
  <tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2"><code><pre>
    FlexView1.Sort(1, "a", "data");
    FlexView1.Sort(1, "aq", "data");
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"></td>
  </tr>
