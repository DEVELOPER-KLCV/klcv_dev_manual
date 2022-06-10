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


A class that displays a spreadsheet that handles tabular data.<br>

The Spread class works in conjunction with the <a href="/package/standard/spreadrow">SpreadRow</a> and <a href="/package/standard/spreadcolumn">SpreadColumn</a> classes.<br>

In order to store the data to be displayed in the spreadsheet, it is necessary to arrange the SpreadRow object and SpreadColomn object in the structure defined under the Spread object.<br>

Since ver5.0, <a href="/package/extension5/sspread">SSpread</a> class that displays high-performance spreadsheets has been added. The SSpread class can realize more advanced functions than the spreadsheet of this class.<br>

**Object Structure**

<a href="/img/Package/Spread.gif" target="_blank">
<img src="/img/Package/Spread.gif" alt="login image"></a><br>


**Screen Display Example** <br>

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std13.files/image002.gif" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


**Printer Output by Doc class** <br>
When the Spread class is used for the printer, the operation differs from that when it is displayed on the screen in the following points.

1. If a cell exists in the column direction beyond the display range, the column will not be printed. <br> <a href="/img/Package/SpreadDisplay.gif" target="_blank"><img src="/img/Package/SpreadDisplay.gif" alt="login image"></a>
2. The <a href="/package/standard/spread/properties/width">Width</a> property of the SpreadColumn class printed in the rightmost column is disabled, and the width is printed up to the display range.
3. If a cell exists at a position that exceeds the display range in the row direction, the row before (above) that row will be printed as it is, but the rows after that will not be printed. However, when data is assigned to the Spread object in CSV format, page breaks are automatically performed when the printable range is exceeded. See the <a href="/package/csvpackage/csvdocument/events/keybreak">CSVDocument.KeyBreak</a> event for more information on this behavior. <br> <a href="/img/Package/Standard-Spread2.PNG" target="_blank"><img src="/img/Package/Standard-Spread2.PNG" alt="login image"></a> 
4. The  <a href="/package/standard/spreadrow/properties/height">Height</a>  property of the SpreadRow class set individually is not reflected. The row heights are all the same.
5. Column headers are always printed in shaded, centered, bold font, and control by the <a href="/package/standard/spread/properties/showlabel">ShowLabel</a>  property is disabled. Also, the line header is not always printed. Control by the <a href="/package/standard/spread/properties/shownumber">ShowNumber</a> property is disabled. 
6. The print properties (<a href="/package/standard/spreadcolumn/properties/suppress">Suppress</a>,  (<a href="/package/standard/spreadcolumn/properties/verticalalign">VerticalAlign</a> properties of the SpreadColumn class) are enabled. <br><br>
   
**Default properties and ValueType**<br>
The default property is <a href="/package/standard/spread/value">Value</a> <br>The ValueType specification is invalid. <br><br>

**Restrictions when visual style is enabled** <br>
◆ LabelBgColor property and NumberBgColor property are invalid because they give priority to the theme background.<br><br>

**Precautions when scaling** <br>
Nothing in particular.