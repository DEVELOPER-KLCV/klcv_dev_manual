---
layout: default

grand_parent: CSVDocument Class
parent: Operators
has_children: false
title: "[ ] << CSV Constant Operator"
nav_order: 1
permalink: /package/csvpackage/csvdocument/operators/1
---
# {{ page.title }}

Loads the CSV constants on the right side of the array object on the left side. By using Record array, SpreadRow, ListItem, etc. on the left side, you can efficiently initialize the object using CSV data.

ListBox initialization example

```
ListBox ListBox1 {
    ListItem ListItem1[];
    ListItem1 << CSV(.Title, .Value) {
    第1営業部,10021
    第2営業部,10022
    製造管理部,20030
    };
}
```

### Object structure that can load CSV data

The array object that can be specified on the left side must have the following structure.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-xt05{background-color:#D9D9D9;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-xt05">Type</th>
    <th class="tg-xt05">Example</th>
    <th class="tg-xt05">Explanation<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">One -dimensional array</td>
    <td class="tg-0lax">String data [ ];<br> </td>
    <td class="tg-0lax">The number of elements in the array corresponds to the number of rows in the CSV data.<br>The number of columns is one, and data itself corresponds to the column.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Two -dimensional equivalent array</td>
    <td class="tg-0lax">Record rec [ ] {<br>    String data1;<br>    String data2;<br>}</td>
    <td class="tg-0lax">The number of elements in the array corresponds to the number of rows in the CSV data.<br>The number of columns is the number of child objects, and data1 and data2 correspond to the columns.<br> </td>
  </tr>
</tbody>
</table>

### Row-wise operation when loading CSV data

If the object on the left side is not explicitly defined by the number of elements in the array, the number of elements in the array will be the same as the number of rows in the CSV data regardless of the number of elements before assignment.

<style type="text/css">
.tg  {border:none;border-collapse:collapse;border-spacing:0;}
.tg td{border-style:solid;border-width:0px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;
  padding:10px 5px;word-break:normal;}
.tg th{border-style:solid;border-width:0px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-9wq8{border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <td class="tg-0pky">Record rec[4] {<br>    Number SURYO;<br>    Number TANKA;<br>}<br>rec &lt;&lt; CSV {<br>1,100<br>2,200<br>2,200<br>1,100<br>3,300  ←切り捨て<br>4,400  ←切り捨て<br>};</td>
    <td class="tg-9wq8">→</td>
    <td class="tg-0pky">
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky"> </th>
    <th class="tg-0pky">SURYO</th>
    <th class="tg-0pky">TANKA</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">[0]</td>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">100</td>
  </tr>
  <tr>
    <td class="tg-0lax">[1]</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">200</td>
  </tr>
  <tr>
    <td class="tg-0lax">[2]</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">200</td>
  </tr>
  <tr>
    <td class="tg-0lax">[3]</td>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">100</td>
  </tr>
</tbody>
</table>    
</td>
  </tr>
</thead>
</table>




```
Record rec[] {
    Number SURYO;
    Number TANKA;
}
rec << CSV {
1,100
2,200
2,200
1,100
};
```

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-73oq"> </th>
    <th class="tg-73oq">SURYO</th>
    <th class="tg-73oq">TANKA</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">[0]</td>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">100</td>
  </tr>
  <tr>
    <td class="tg-0lax">[1]</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">200</td>
  </tr>
  <tr>
    <td class="tg-0lax">[2]</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">200</td>
  </tr>
  <tr>
    <td class="tg-0lax">[3]</td>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">100</td>
  </tr>
</tbody>
</table>

If the object on the left side is explicitly defined by the number of elements in the array, it will be treated as a fixed-length array in CSV data assignment. The number of elements in the array does not change regardless of the number of rows in the CSV data.
If there are more CSV data rows than there are elements, the CSV data rows that exceed the number of elements will be truncated. If the CSV data has a small number of rows, the values of subsequent array elements do not change and retain the values before loading the CSV data.

For  Number of elements in the array < The number of rows of CSV data

```
Record rec[4] {
    Number SURYO;
    Number TANKA;
}
rec << CSV {
1,100
2,200
2,200
1,100
3,300  ←切り捨て
4,400  ←切り捨て
};
```

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-73oq"> </th>
    <th class="tg-73oq">SURYO</th>
    <th class="tg-73oq">TANKA</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">[0]</td>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">100</td>
  </tr>
  <tr>
    <td class="tg-0lax">[1]</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">200</td>
  </tr>
  <tr>
    <td class="tg-0lax">[2]</td>
    <td class="tg-0lax">2</td>
    <td class="tg-0lax">200</td>
  </tr>
  <tr>
    <td class="tg-0lax">[3]</td>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">100</td>
  </tr>
</tbody>
</table>

Number of elements in the array > Number of rows of CSV data

```

Record rec[6] {
    Number SURYO;
    Number TANKA;
}
    :
rec << CSV {
1,100
2,200
2,200
1,100
};
```


