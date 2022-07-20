---
layout: default

grand_parent: CSVDocument Class
parent: Events
has_children: false
title: CSVDocument.KeyBreak Event
nav_order: 3
permalink: /package/csvpackage/csvdocument/events/keybreak
---
# {{ page.title }}

When key break is performed before or after the array data currently being focused on, if a value is specified for the BreakKey property (<a href="/package/standard/spreadcolumn/properties/breakkey">SpreadColumn.BreakKey</a> property, etc.) of the object corresponding to the column by loading CSV data into the array object to be printed, the KeyBreak event will occur according to the following rules.The KeyBreak event does not occur for objects that do not have the BreakKey property or for classes that are not printed.

If the value of the BreakKey property is positive,
compare the row of interest to the previous row before assigning it to an array element. If the result of the comparison is different, the row just before the assigned row is judged to be the key break.

If the value of the BreakKey property is negative,
assign the row of interest to the array element and then compare it to the one row just before the assigned row. If the result of the comparison is different, the currently paying attention row is judged to be the key break.

If multiple items are determined to be keybreaks at the same time, the KeyBreak event will occur only for the object with the largest absolute value of the BreakKey property. If the values ​​of the BreakKey property are the same, the KeyBreak event will occur on the previously defined object (the leftmost column in the <a href="/package/standard/spread/">Spread</a> class).

Example1
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-8fdo{background-color:#CFC;text-align:left;vertical-align:top}
.tg .tg-qri1{background-color:#CFF;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-145f{background-color:#FF9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-hw7o{background-color:#FF0;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05"> </th>
    <th class="tg-xt05">Item1<br>BreakKey = 1</th>
    <th class="tg-xt05">Item2<br>BreakKey = 2</th>
    <th class="tg-xt05">Item3<br>BreakKey = 3</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">1st line</td>
    <td class="tg-0lax">"AAA"</td>
    <td class="tg-0lax">"XXX"<img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/csv/csv1e3.files/image001.gif" width="29" height="13"></td>
    <td class="tg-0lax">"111"</td>
  </tr>
  <tr>
    <td class="tg-0lax">2nd line</td>
    <td class="tg-0lax">"AAA"</td>
    <td class="tg-145f">"YYY"</td>
    <td class="tg-0lax">"111"<img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/csv/csv1e3.files/image001.gif" width="29" height="13"></td>
  </tr>
  <tr>
    <td class="tg-0lax">3rd line</td>
    <td class="tg-qri1">"BBB"</td>
    <td class="tg-hw7o">"ZZZ"</td>
    <td class="tg-8fdo">"222"</td>
  </tr>
  <tr>
    <td class="tg-0lax">4th line</td>
    <td class="tg-qri1">"BBB"</td>
    <td class="tg-hw7o">"ZZZ"</td>
    <td class="tg-8fdo">"222"</td>
  </tr>
</tbody>
</table>

In this example, the KeyBreak event occur as follows:

After setting the data in the first row to the array, the KeyBreak event occur at Item2[0].
After setting the data in the second row to the array, the KeyBreak event occur at Item3[1].

Example2
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-8fdo{background-color:#CFC;text-align:left;vertical-align:top}
.tg .tg-qri1{background-color:#CFF;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-145f{background-color:#FF9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-hw7o{background-color:#FF0;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05"> </th>
    <th class="tg-xt05">Item1<br>BreakKey = -1</th>
    <th class="tg-xt05">Item2<br>BreakKey = -2</th>
    <th class="tg-xt05">Item3<br>BreakKey = -3</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">1st line</td>
    <td class="tg-0lax">"AAA"</td>
    <td class="tg-0lax">"XXX"</td>
    <td class="tg-0lax">"111"</td>
  </tr>
  <tr>
    <td class="tg-0lax">2nd line</td>
    <td class="tg-0lax">"AAA"</td>
    <td class="tg-145f">"YYY"<img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/csv/csv1e3.files/image001.gif" width="29" height="13"></td>
    <td class="tg-0lax">"111"</td>
  </tr>
  <tr>
    <td class="tg-0lax">3rd line</td>
    <td class="tg-qri1">"BBB"</td>
    <td class="tg-hw7o">"ZZZ"</td>
    <td class="tg-8fdo">"222"<img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/csv/csv1e3.files/image001.gif" width="29" height="13"></td>
  </tr>
  <tr>
    <td class="tg-0lax">4th line</td>
    <td class="tg-qri1">"BBB"</td>
    <td class="tg-hw7o">"ZZZ"</td>
    <td class="tg-8fdo">"222"</td>
  </tr>
</tbody>
</table>

In this example, the KeyBreak event occur as follows:

After setting the data in the second row to the array, the KeyBreak event occur at Item2[1].
After setting the data in the third row to the array, the KeyBreak event occur at Item3[2].

In the event handler triggered by the KeyBreak event, you can get the index value of the broken row by the CurrentIndex of the event object passed to the event handler. By assigning a new value to CurrentIndex, you can change the assignment position of subsequent data.

Example of advancing an insert line by one line
```
   Function OnKeyBreak(e) {
    e.CurrentIndex++;
    }
```


When the CurrentIndex is changed inside the event handler or the array object to be assigned CSV data is changed, the result is a sequence of data that becomes a key break condition in the subsequent assignment of CSV data. However, this operation does not raise the KeyBreak event. The key break decision is always based on the value of the original CSV data.

Example3

```
Function OnKeyBreak(e) {
    rec.insert(1);
    rec[e.CurrentIndex+1].item1 = "合計";
    rec[e.CurrentIndex+1].item2 = goukei;
    e.CurrentIndex++;
}
```

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-8fdo{background-color:#CFC;text-align:left;vertical-align:top}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05"> </th>
    <th class="tg-xt05">Item1<br>BreakKey = 1</th>
    <th class="tg-xt05">Item2<br>BreakKey = 0</th>
    <th class="tg-xt05">Item3<br>BreakKey = 0</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">1st line</td>
    <td class="tg-0lax">"AAA"</td>
    <td class="tg-0lax">"XXX"</td>
    <td class="tg-0lax">111</td>
  </tr>
  <tr>
    <td class="tg-0lax">2nd line</td>
    <td class="tg-0lax">"AAA"</td>
    <td class="tg-0lax">"YYY"</td>
    <td class="tg-0lax">222</td>
  </tr>
  <tr>
    <td class="tg-8fdo">3rd line</td>
    <td class="tg-8fdo"> </td>
    <td class="tg-8fdo">" Total "</td>
    <td class="tg-8fdo">333</td>
  </tr>
  <tr>
    <td class="tg-0lax">4th line</td>
    <td class="tg-0lax">"BBB"</td>
    <td class="tg-0lax">"ZZZ"</td>
    <td class="tg-0lax">555</td>
  </tr>
</tbody>
</table>

In this example, the KeyBreak event that occurs in the second line of item1 executes the event handler shown in the above example and creates the third line. Subsequent CSV data creates the 4th line, and as the result, data changes in the 3rd and 4th lines of item1, but this change does not cause the KeyBreak event again.
<br><br><small><span style="color:blue">Not supported in Mobile</span></small>