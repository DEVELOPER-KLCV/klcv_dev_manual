---
layout: default

parent: 2. Standard Package
has_children: true

title: Spread Class
nav_order: 24
permalink: /package/standard/spread

---


# {{ page.title }}
<br>

<a href="/img/Package/Standard-Spread.PNG" target="_blank">
<img src="/img/Package/Standard-Spread.PNG" alt="login image"></a>


A class that displays a spreadsheet that handles tabular data.<br><br>

The Spread class works in conjunction with the SpreadRow and SpreadColomn classes.<br>

In order to store the data to be displayed in the spreadsheet, it is necessary to arrange the SpreadRow object and SpreadColomn object in the structure defined under the Spread object.<br><br>

Since ver5.0, SSpread class that displays high-performance spreadsheets has been added. The SSpread class can realize more advanced functions than the spreadsheet of this class.

**Object Structure**

<a href="/img/Package/Spread.gif" target="_blank">
<img src="/img/Package/Spread.gif" alt="login image"></a><br>


**Screen Display Example** <br>

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std13.files/image002.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}"></a> <br>


**Printer Output by Doc class** <br>

When the Spread class is used for the printer, the operation differs from that when it is displayed on the screen in the following points.


<html>
<body>

<h2>Ordered List with Numbers</h2>

<ol type="1">
  <li>If a cell exists in the column direction beyond the display range, the column will not be printed. </li>
  <li>The Width property of the SpreadColumn class printed in the rightmost column is disabled, and the width is printed up to the display range.</li>
  <li>If a cell exists at a position that exceeds the display range in the row direction, the row before (above) that row will be printed as it is, but the rows after that will not be printed. However, when data is assigned to the Spread object in CSV format, page breaks are automatically performed when the printable range is exceeded. See the CSVDocument.KeyBreak event for more information on this behavior.</li>
</ol>  

</body>
</html>
   

   