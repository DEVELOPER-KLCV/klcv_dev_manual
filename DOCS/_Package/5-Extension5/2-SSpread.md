---
layout: default

parent: 5. Extension5 Package
has_children: true

title: SSpread Class
nav_order: 2
permalink: /package/extension5/sspread

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}

# {{ page.title }}

<a href="/img/Package/Ext5-SSpread.PNG" target="_blank">
<img src="/img/Package/Ext5-SSpread.PNG" alt="login image"></a>

A class that displays high-performance spreadsheets.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext5/ext_sspread.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**<br>
Not subject to printing.

**Default properties and ValueType**<br>
There are no default properties. The value type specification is invalid.

**Character Code**<br>
In this class, the basic character code is treated as Unicode, and the properties and methods that handle character strings are UString type with some exceptions.

If you set an object of type String, it will be automatically converted to type UString before processing.

When specifying the number of characters and the position of characters, it is in character units without distinction such as full-width / half-width.

**SSpread class-specific property execution order specification**<br>

In normal CRS execution, the properties set in the script are reflected on the GUI side after the execution of the series of scripts is completed.

Therefore, the setting order of properties is not related to the reflection of GUI, and conversely, when referencing properties, the state of GUI is not reflected in real time.

However, the SSpread class is designed with a strong awareness of porting from client-server type applications created with Visual Basic, and is executed with different behavior rules from other classes.

Setting and reading properties is accessed in real time in the GUI and executed in the order in which they are written, including methods.


(Description example)

```
Col = 2;
Row = 3;
BgColor = $BLUE;
Col = 4;
Row = 5;
BgColor = $RED;
```

In normal CRS execution, only Col = 4, Row = 5, BgColor = $ RED described later are valid, but in SSpread class, Col = 2, Row = 3, BgColor = $ BLUE are executed as described, and In addition, Col = 4, Row = 5, BgColor = $ RED are executed.

Therefore, the order in which the properties are written directly affects the execution speed.

Generally, the speed decreases as the number of target cells increases, so it is more efficient to execute the property method that is reflected in the entire spreadsheet at the stage where the cell data is as small as possible.

**Col, Row, Col2, Row2, BlockMode properties**<br>
The <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a>, <a href="/package/extension5/sspread/properties/col2">Col2</a>, and <a href="/package/extension5/sspread/properties/row2">Row2</a> properties are used to set the scope of processing before performing various processing on the spreadsheet.

Targets for which these properties need to be preset include the <a href="/package/extension5/sspread/properties/backcolor">BackColor</a>, <a href="/package/extension5/sspread/properties/forecolor">ForeColor</a>, <a href="/package/extension5/sspread/properties/fontbold">FontBold</a>, <a href="/package/extension5/sspread/properties/fontitalic">FontItalic</a>, <a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a>, <a href="/package/extension5/sspread/properties/lock">Lock</a>, and <a href="/package/extension5/sspread/properties/formula">Formula</a> properties.

| Processing object        | Properties to set                             |
|--------------------------|-----------------------------------------------|
| Cell                     | Col , Row                                     |
| Column (1 column)        | Col , Row ( -1 )                              |
| Column range             | Col , Col2                                    |
| Column header (1 column) | Col , Row ( 0 )                               |
| Whole column header      | Col ( -1 ), Row ( 0 )                         |
| Row                      | Row , Col ( -1 )                              |
| Range of rows            | Row , Row2                                    |
| Row header (1 column)    | Col ( 0 ), Row                                |
| Whole row header         | Col , Row ( -1 )                              |
| Cell block               | Col , Row , Col2 , Row2 , BlockMode ( $TRUE ) |
| Entire spreadsheet       | Col ( -1 ), Row ( -1 )                        |

Set <a href="/package/extension5/sspread/properties/blockmode">BlockMode</a> to $TRUE to enable the Col2, Row2 properties to specify cell blocks.

If you leave BlockMode at $TRUE after setting it to a cell block, it may affect the unintended range in the subsequent processing, so it is recommended to return it to $FALSE after use.

If you specify multiple cells with different values and refer to the values, the value of one representative cell will be returned in principle. To ensure that you get the value of a particular cell, specify the cell clearly in the Col and Row properties before referencing.

**This class's unique color handling (#RRGGBB format)**<br>
Apart from the standard color constants ($BLACK, $FF0000, etc.), any color can be used in this class.

Color information is represented by a character string in the following format.
```
"#RRGGBB"
```
1st character: #

2nd and 3rd characters (RR): Hexagonal number (00 to FF) representing the red component

4th and 5th characters (GG): Hexagonal number representing the green component (00 to FF)

6th and 7th characters (BB): Hexagonal number (00 to FF) representing the blue component<br>
(Example)<br> Orange color

For the colors defined in the color constants, the color constants take precedence even if the string format is specified.

Specifying $ STD sets the standard color.

**Index Property**<br>
Some properties get and set the value by specifying the index number of the target data. (Example: <a href="/package/extension5/sspread/properties/colwidth">ColWidth</a>, <a href="/package/extension5/sspread/properties/rowheight">RowHeight</a> property, etc.)

```
/* 取得例 */
var w = ColWidth(5);
var h = RowHeight(7);
/* 設定例 */
ColWidth(5) = w + 10;
RowHeight(7) = h + 10;
```

Notice that the index number is enclosed in (n) (round brackets) instead of the [n] (square brackets) that represent the array.

The substance of these properties is a method, and by passing an index number as an argument of the method, it behaves like a property.

(Displayed as a method on Biz / Desiger)

In this manual, properties with such a function are called "index properties" and are treated as properties.


**Restriction of property setting by reference operator (& =)**<br>
The "reference operator", which is an operator peculiar to Biz / Browser, automatically assigns the changed value to the left side when the right side of the assignment expression is changed.

(Example)
```
Width &= ^.Width - 10;
Height &= ^.Height - 10;
```

However, there are many properties in this class that can be changed to affect the values of other properties or behave differently depending on the order in which they are set.

When a reference operator is used for such a property, the intended result is difficult to obtained because the processing target of the assignment destination (left side) and the value of the reference destination (right side) may differ depending on the state of other properties. 

Properties whose "& =" column in the <a href="/package/extension5/sspread/properties">Property List</a> is "x" are targeted.

(A typical example is a property that presets the Col and Row properties.)

**Do not use** these properties on either the left or right side of the reference operator.

(Example that cannot be used)
```
Col = 2;
Row = 3;
BackColor & = ^. Label1.BgColor; / * Specify on the left side * /
Col = 4;
Row = 5;
^ .Label1.BgColor = $ RED; / * The reference operator changes the background color of columns 4 rows 5 cells * /
 
Col = 6;
Row = 7;
^ .Label2.BgColor & = BackColor; / * Specify on the right side * /
Col = 8;
Row = 9;
BackColor = $ GREEN; / * The reference operator changes the background color of Label2 * /
```

Note that these properties are excluded from the property view of Biz / Designer so that they cannot be set, so specify them directly in the CRS program.


**Limits on fonts applied to cell blocks**<br>
If you use the  <a href="/package/extension5/sspread/properties/fontbold">FontBold</a>,<a href="/package/extension5/sspread/properties/fontface">FontFace</a>, <a href="/package/extension5/sspread/properties/fontitalic">FontItalic</a>, <a href="/package/extension5/sspread/properties/fontkind">FontKind</a>, <a href="/package/extension5/sspread/properties/fontname">FontName</a>, <a href="/package/extension5/sspread/properties/fontsize">FontSize</a>, <a href="/package/extension5/sspread/properties/fontstrikethru">FontStrikethru</a>, and <a href="/package/extension5/sspread/properties/fontunderline">FontUnderline</a> properties and set <a href="/package/extension5/sspread/properties/blockmode">BlockMode</a> to $TRUE to apply the settings to a cell block, the font settings for each cell will be discarded and the font will be recreated based on the cell pointed to by the <a href="/package/extension5/sspread/properties/col">Col</a> and <a href="/package/extension5/sspread/properties/row">Row</a> properties.

In other words, if you make a cell "bold" and then apply "oblique" to the cell block that contains that cell, the "bold" will be canceled.

When setting fonts, first make common settings from a large range, and then make individual settings.

**Get and set the value for each cell data type**<br>
Depending on the cell data type set in the CellType property, the cell value can be obtained and set as follows.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0ss8{background-color:#c0c0c0;border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;
  vertical-align:top}
.tg .tg-j5n6{border-color:inherit;font-family:Arial, Helvetica, sans-serif !important;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0ss8">Cell data type</th>
    <th class="tg-0ss8">Data / status</th>
    <th class="tg-0ss8"><a href="/package/extension5/sspread/properties/text">Text</a> property</th>
    <th class="tg-0ss8"><a href="/package/extension5/sspread/properties/value">Value</a> property</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-j5n6">Text type</td>
    <td class="tg-j5n6">-</td>
    <td class="tg-j5n6">String</td>
    <td class="tg-j5n6">String</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Label type</td>
    <td class="tg-j5n6">-</td>
    <td class="tg-j5n6">String</td>
    <td class="tg-j5n6">String</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Date type</td>
    <td class="tg-j5n6">"2011/04/27"</td>
    <td class="tg-j5n6">"2011/04/27"</td>
    <td class="tg-j5n6">"20110427"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Momentary</td>
    <td class="tg-j5n6">"11:25:03 pm"</td>
    <td class="tg-j5n6">"11:25:03 pm"</td>
    <td class="tg-j5n6">"232503"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Numeric type</td>
    <td class="tg-j5n6">"10,000.00"</td>
    <td class="tg-j5n6">"10,000.00"</td>
    <td class="tg-j5n6">"10000.00"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Currency type</td>
    <td class="tg-j5n6">"\10,000.00"</td>
    <td class="tg-j5n6">"\10,000.00"</td>
    <td class="tg-j5n6">"10000.00"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Percentage type</td>
    <td class="tg-j5n6">"15%"</td>
    <td class="tg-j5n6">"15%"</td>
    <td class="tg-j5n6">"0.15"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Exponential</td>
    <td class="tg-j5n6">"2.22E+05"</td>
    <td class="tg-j5n6">"2.22E+05"</td>
    <td class="tg-j5n6">"222222"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Mask type</td>
    <td class="tg-j5n6">"22-45-76"</td>
    <td class="tg-j5n6">"22-45-76"</td>
    <td class="tg-j5n6">"224576"</td>
  </tr>
  <tr>
    <td class="tg-j5n6" rowspan="3">Command button</td>
    <td class="tg-j5n6">Being pressed</td>
    <td class="tg-j5n6">"1"</td>
    <td class="tg-j5n6">"1"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Not pressed</td>
    <td class="tg-j5n6">"0"</td>
    <td class="tg-j5n6">"0"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Not set</td>
    <td class="tg-j5n6">blank text column</td>
    <td class="tg-j5n6">"0"</td>
  </tr>
  <tr>
    <td class="tg-j5n6" rowspan="4">Checkbox</td>
    <td class="tg-j5n6">Ticked</td>
    <td class="tg-j5n6">"1"</td>
    <td class="tg-j5n6">"1"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Unticked</td>
    <td class="tg-j5n6">"0"</td>
    <td class="tg-j5n6">"0"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Gray state</td>
    <td class="tg-j5n6">"2"</td>
    <td class="tg-j5n6">"2"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Not set</td>
    <td class="tg-j5n6">blank text column</td>
    <td class="tg-j5n6">"0"</td>
  </tr>
  <tr>
    <td class="tg-j5n6">Combo box</td>
    <td class="tg-j5n6">-</td>
    <td class="tg-j5n6">String data of the selected element</td>
    <td class="tg-j5n6">Index of selected element<br>(Blank character string when not selected)</td>
  </tr>
</tbody>
</table>

**Precautions for specifying the range based on the lower and upper limits**<br>

Properties that specify a range of values, such as <a href="/package/extension5/sspread/properties/typenumbermin">TypeNumberMin</a> and <a href="/package/extension5/sspread/properties/typenumbermax">TypeNumberMax</a>, can limit input operations, but do not guarantee that the values will be within the range. Incorrect values may be set temporarily by input operations, or incorrect values may be set from the CRS script.

The <a href="/package/extension5/sspread/events/editerror">EditError</a> event is raised when an invalid value is set by an input operation. If want to make sure that the value is checked, control it with a CRS script.

**Notes on property references in event handlers**<br>
Biz / Browser events are executed sequentially after being accumulated in the event queue. Therefore, there is no guarantee that the timing and order of events will always be the same.

Even for events that occur in this class, the value of the property referenced in the event handler may differ depending on the execution status. For example, the <a href="/package/extension5/sspread/events/leavecell">LeaveCell</a>  event is generated by moving the active cell, but it is uncertain whether the value before or after the move can be obtained when the <a href="/package/extension5/sspread/properties/activecol">ActiveCol</a> or <a href="/package/extension5/sspread/properties/activerow">ActiveRow</a> property is referenced in the OnLeaveCell event handler.

Events of this class are passed relevant information as child objects of event handler arguments (Event objects), so be sure to use that information.

```
Function OnLeaveCell(e) {
    ^.Label1.Value = ActiveCol; /* variable */
    ^.Label2.Value = ActiveRow; /* variable */
    ^ .Label3.Value = e.Col;      / * Column number before moving * /
    ^ .Label4.Value = e.Row;      / * Row number before moving * /
    ^ .Label5.Value = e.NewCol;   / * Column number after move * /
    ^ .Label6.Value = e.NewRow;   / * Moved row number * /
}
```

**Inherited property for each cell data type**<br>
The <a href="/package/extension5/sspread/properties/celltype">CellType</a> property and properties whose name starts with "Type" set the cell data type. These properties are stored for the last setting for each cell data type, and are inherited the next time they are set for a cell with the same data type. See the <a href="/package/extension5/sspread/properties/celltype">CellType</a> property for more information.


**Standard keyboard operation and KeyDown event**<br>
The spreadsheet can be operated with the following keys.


| Key                    | Action                                                                                                          |
|------------------------|-----------------------------------------------------------------------------------------------------------------|
| Arrow keys             | Move active cell Extend the selection with the Shift key                                                        |
| PageUp , PageDown keys | Move the active cell up or down on a page-by-page basis Move left or right with Ctrl key                        |
| Home , End key         | Move active cell to first or last cell in row Use the Ctrl key to move to the first and last cells of the whole |
| Tab key                | Set in <a href="/package/extension5/sspread/properties/processtab">ProcessTab</a>  property                                                                                      |
| Space key              | Select a line with the Ctrl key Select a column with the Shift key Select all with Ctrl + Shift                 |
| Enter key              | Set by <a href="/package/extension5/sspread/properties/editenteraction">EditEnterAction</a> property                                                                                 |
| Esc key                | Cancel selection etc.                                                                                           |
| Delete key             | Set with <a href="/package/extension5/sspread/properties/processdelete">ProcessDelete</a> property                                                                                 |

If set the <a href="/package/extension5/sspread/properties/autoclipbord">AutoClipbord</a> property to $TRUE, the following key operations also can be used.

| Key                        | Action |
|----------------------------|--------|
| Ctrl +'C' , Ctrl + Insert  | Copy   |
| Ctrl +'X' , Shift + Delete | Cut    |
| Ctrl +'V' , Shift + Insert | Paste  |


The above key does not generate the <a href="/package/extension5/sspread/events/keydown">KeyDown</a> event of the parent Form when pressed. Specifying <a href="/package/extension5/sspread/properties/altkey">AltKey</a> properties such as Button on the same Form is also invalid.

Other keys will raise the KeyDown event of the parent Form if they are not used to edit the data. Control by key operation should be performed by the OnKeyDown event handler of the parent Form.


**Import/Export function in Excel**<br>
SSpread is equipped with methods for reading from Excel format files and outputting to Excel format.

This function tries to match the cell information handled by SSpread with the cell information handled by Excel as much as possible, but please note that the input / output results do not exactly match because there are differences in the functions that can be handled by each.

Also, macros (VBA), graphs, and other images cannot be input or output with SSpread.

Please note that if the file has an extremely large size or a large number of formulas, it will take a very long time to import / export, and the process may slow down or stop (no response).

&nbsp; &nbsp; ***Correspondence of ruled line during output***
&nbsp; &nbsp; The relationship between the ruled line specified by SSpread and the ruled line output is as follows.




































































































































































































































































































































































































































