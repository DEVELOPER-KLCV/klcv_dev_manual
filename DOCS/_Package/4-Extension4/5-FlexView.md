---
layout: default

parent: 4. Extension4 Package
has_children: true

title: FlexView Class
nav_order: 5
permalink: /package/extension4/flexview

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-FlexView.PNG" target="_blank">
<img src="/img/Package/Ext4-FlexView.PNG" alt="login image"></a>

This class is used to display tabular data.

It is similar to the Spread class and ListView class, but it can be grouped according to the contents of the data and displayed like a split merge of cells. In addition, text boxes and buttons can be placed directly in the cells.

The FlexView class, unlike other tabular classes, has no corresponding object for each cell. Like CSVDocument, individual cells are managed as internal data in FlexView and need to be accessed through methods. Even if the number of rows is large, the number of objects generated is small, so you can handle more rows than Spread or ListView.

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexview.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**<br>
 Not subject to printing.


**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/flexview/flexview/properties/rowposition">RowPosition</a>. The ValueType specification is invalid.

**FlexView Overview**<br>
The FlexView object is a composite object that does not work by itself, and it uses FlexRecord and FlexItem derived classes placed underneath.

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexview.files/image002.gif" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

Place one FlexRecord under FlexView. You cannot have multiple FlexRecords or an array of FlexRecords. Note that FlexRecord is an object that defines how a table row is displayed, not an object that represents the row itself.

The following objects derived from <a href="/package/extension4/flexview/flexitem">FlexItem</a> can be placed under  <a href="/package/extension4/flexview/flexrecord">FlexRecord</a>. These objects define the display form of the column and the initial value of the cell, not the object that represents the cell itself.

| Class           | Cell accessor class | Description                                                                               |
|-----------------|---------------------|-------------------------------------------------------------------------------------------|
|[FlexRowSet](/package/extension4/flexview/flexrowset)   | None                | Display the lower FlexItems in multiple lines.                                            |
|[FlexColumnSet](/package/extension4/flexview/flexcolumnset)   | None                | Display the lower FlexItems in multiple columns.                                          |
|[FlexHeader](/package/extension4/flexview/flexheader)      |[FlexHeaderCell](/package/extension4/flexview/flexheadercell)       | Line header                                                                               |
|[FlexGroupHeader](/package/extension4/flexview/flexgroupheader) |[FlexGroupHeaderCell](/package/extension4/flexview/flexgroupheadercell)  | Grouping line header                                                                      |
|[FlexTreeHeader](/package/extension4/flexview/flextreeheader)  |[FlexTreeHeaderCell](/package/extension4/flexview/flextreeheadercell)  | Tree display line header                                                                  |
|[FlexLabel](/package/extension4/flexview/flexlabel)       |[FlexLabelCell](/package/extension4/flexview/flexlabelcell)       | Display cells like labels                                                                 |
|[FlexIndentLabel](/package/extension4/flexview/flexindentlabel) |[FlexIndentLabelCell](/package/extension4/flexview/flexindentlabelcell) | Indent travel                                                                             |
|[FlexButton](/package/extension4/flexview/flexbutton)      | [FlexButtonCell](/package/extension4/flexview/flexbuttoncell)      | Display cells like buttons. It is possible to click.                                      |
|[FlexCheckButton](/package/extension4/flexview/flexcheckbutton)  | [FlexCheckButtonCell](/package/extension4/flexview/flexcheckbuttoncell) | Displays cells like checkboxes. You can change the selection status by clicking.          |
|[FlexTextBox](/package/extension4/flexview/flextextbox)     |[FlexTextBoxCell](/package/extension4/flexview/flextextboxcell)     | Display the cell like a text box. Editing by key input is possible.                       |
|[FlexListBox](/package/extension4/flexview/flexlistbox)     |[FlexListBoxCell](/package/extension4/flexview/flexlistboxcell)     | Display the cells like a pull-down list. You can change the selection status by clicking. |

The class whose class name is described in the cell accessor class is a class derived from the FlexData class and displays the data corresponding to one column of table data in the cell. Classes marked "None" are not related to table data.

The FlexRowSet and FlexColumnSet classes define the placement of cells and place lower FlexItems in the column or row direction. You can place a derived class of FlexItem at the lower level, and you can make any division by placing multiple FlexRowSet or FlexColumnSet in the lower hierarchy.

```
FlexRecord R {
    FlexRowSet Row1 {
        FlexColumnSet Col1 {
            FlexLabel Label1;
            FlexLabel Label2;
            FlexLabel Label3;
        }
        FlexColumnSet Col2 {
            FlexLabel Label4;
            FlexLabel Label5;
            FlexLabel Label6;
        }
    }
}
```

{% assign img3 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexview.files/image003.png" %}

<a href="{{ img3 }}" target="_blank"> <img src="{{ img3 }}" alt="{{img3}}"></a>

**FlexData and Cell Relationship**

The data displayed in the cell is configured by referring to the derived object from the FlexData class placed under the FlexRecord object when the row is generated by the FlexView.InsertRow method etc. and managed as the internal data of the FlexView object.

The value specified for FlexLabel.Value etc. is copied when the cell is configured and maintained as a separate instance from FlexLabel.Value. Therefore, updating the values in individual cells does not affect the FlexLabel object.

FlexItem layout structure<br>
{% assign img4 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexview.files/image004.gif" %}

<a href="{{ img4 }}" target="_blank"> <img src="{{ img4 }}" alt="{{img4}}"></a>


Results displayed by InsertRow

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-4ab0{background-color:#CFF;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-4ab0">①</th>
    <th class="tg-4ab0" rowspan="2">③</th>
    <th class="tg-4ab0" rowspan="2">④</th>
  </tr>
  <tr>
    <th class="tg-4ab0">②</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky"> </td>
    <td class="tg-0pky" rowspan="2"> <br></td>
    <td class="tg-0pky" rowspan="2"> <br></td>
  </tr>
  <tr>
    <td class="tg-0pky"> </td>
  </tr>
  <tr>
    <td class="tg-4ab0"> </td>
    <td class="tg-4ab0" rowspan="2"> <br></td>
    <td class="tg-4ab0" rowspan="2"> <br></td>
  </tr>
  <tr>
    <td class="tg-4ab0"> </td>
  </tr>
</tbody>
</table>


In this example, one FlexRowSet and four FlexLabels are placed under FlexRecord. Since FlexRowSet is not derived from the FlexData class, no corresponding cell will be created. Since FlexLabel is a class derived from FlexData, 4 cells (1) to (4) corresponding to 4 FlexLabels are generated.

Some properties such as Value value and FgColor set in FlexLabel are copied to these generated cells and maintained for each cell. Also, other properties such as VerticalAlign and BorderStyle are not copied, they are referenced and shared by all cells.

Note that properties that are not managed on a cell-by-cell basis cannot be changed on a per-cell basis. For example, the display style of the cell border specified by FlexLebel.BorderStyle cannot be changed on a cell-by-cell basis. Which properties are managed on a cell-by-cell basis and which properties are shared depends on the class. Please refer to the document of each class for details.


**Accessor Object**

Since cells are not objects, it cannot directly manipulate individual cells, but a derived class of the FlexCell class is defined as an accessor to the cell. An accessor is a kind of pointer, and operations on the accessor are transmitted to the cell pointed to by the accessor. For example, if you change the BgColor of FlexLabelCell, the accessor of a cell composed of FlexLabel, the background color of the cell pointed to by FlexLabelCell will change.

Since the accessor is not the cell itself, all operations on the accessor do not affect the cell. For example, you can delete an accessor with the Delete method, but it will not delete the cell. Also, the accessor object is preserved even if the cell pointed to by the accessor is lost, such as with the FlexView.DeleteRow method.


**Creation of Accessor**

Accessors cannot be generated directly from a script, they are generated as return values for the <a href="/package/extension4/flexview/flexview/methods/getrow">FlexView.GetRow</a>, <a href="/package/extension4/flexview/flexview/methods/insertrow">FlexView.InsertRow</a>, and <a href="/package/extension4/flexview/flexview/methods/deleterow">FlexView.DeleteRow</a> methods, and as child objects of the <a href="/package/extension4/flexview/flexrow">FlexRow</a> object that can be obtained as additional data for various events.

FlexRow points to a specific row in the table and has a FlexCell derived object in its child object that has the same name as the FlexData derived object from which the cell originated. Each FlexCell derived object points to the corresponding cell in the row that FlexRow points to.


Example accessor returned by InsertRow

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-4ab0{background-color:#CFF;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-qri1{background-color:#CFF;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-4ab0"> </th>
    <th class="tg-4ab0" rowspan="2"> <br></th>
    <th class="tg-4ab0" rowspan="2"> <br></th>
  </tr>
  <tr>
    <th class="tg-qri1"> </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">A</td>
    <td class="tg-0lax" rowspan="2">C</td>
    <td class="tg-0lax" rowspan="2">D</td>
  </tr>
  <tr>
    <td class="tg-0lax">B</td>
  </tr>
  <tr>
    <td class="tg-qri1"> </td>
    <td class="tg-qri1" rowspan="2"> <br></td>
    <td class="tg-qri1" rowspan="2"> <br></td>
  </tr>
  <tr>
    <td class="tg-qri1"> </td>
  </tr>
</tbody>
</table>

```
var row = FlexView1.InsertRow(1,1);
```

The structure of the FlexRow returned to row. Row points to the new row you inserted.


{% assign img5 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexview.files/image005.gif" %}

<a href="{{ img5 }}" target="_blank"> <img src="{{ img5 }}" alt="{{img5}}"></a>

When row.A is updated, it will be reflected in the cell corresponding to A.

```
row.A.BgColor = $RED;
row.C.Value = "123";
```

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-4ab0{background-color:#CFF;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-qri1{background-color:#CFF;text-align:left;vertical-align:top}
.tg .tg-6y22{background-color:#F00;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-4ab0"> </th>
    <th class="tg-4ab0" rowspan="2"> <br></th>
    <th class="tg-4ab0" rowspan="2"> <br></th>
  </tr>
  <tr>
    <th class="tg-qri1"> </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-6y22">A</td>
    <td class="tg-0lax" rowspan="2">123</td>
    <td class="tg-0lax" rowspan="2">D</td>
  </tr>
  <tr>
    <td class="tg-0lax">B</td>
  </tr>
  <tr>
    <td class="tg-qri1"> </td>
    <td class="tg-qri1" rowspan="2"> <br></td>
    <td class="tg-qri1" rowspan="2"> <br></td>
  </tr>
  <tr>
    <td class="tg-qri1"> </td>
  </tr>
</tbody>
</table>

**Constraints on Accessor Usage**

All accessors must have unique names because they are generated as direct children of FlexRow. On the other hand, FlexItem can be defined with a hierarchy by making it a child of FlexRowSet and FlexColumnSet, but if there are multiple FlexData derived objects with the same name at that time, the object with the same name defined after the second one. You will no longer be able to use the corresponding accessor by name.

{% assign img6 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexview.files/image006.gif" %}

<a href="{{ img6 }}" target="_blank"> <img src="{{ img6 }}" alt="{{img6}}"></a>

FlexData Structure       &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;          Corresponding Accessor Structure


In the case of this example, subsequent LabelA and LabelB (yellow part) cannot be operated by name.

If you use the GetColumn and GetHeaderColumn methods provided in FlexRow, you can get FlexCell by position instead of name. When operating LabelA and LabelB after that, it will be 

```
var lb_a = row.GetColumn(2); /* 3列目 LabelA */
var lb_b = row.GetColumn(3); /* 4列目 LabelB */
```

but if the display position is changed, it will be necessary to correct the program accordingly.

Also, when loading a named CSV, no data will be assigned to subsequent LabelA and LabelB.

Many of these restrictions occur when using the same column name. Try to give each column a unique name whenever possible.


**Effective Range of Accessor Usage**
 
Accessors are generated dependent on the FlexRow object that points to the row and work with the internal FlexRow object to actually access the cell. Therefore, the accessor object cannot work if the FlexRow object is lost. Always maintain a FlexRow object while using the accessor.


**Constraints on Display Order and Cursor Movement Order**
 
FlexData-derived classes placed under FlexRecord are displayed from left to right and top to bottom in their definition order. Also, the left and right arrow keys move the cursor in the defined order. It cannot be displayed in a different order from the definition order, or the cursor movement order cannot be changed.

**Constraints Layout of FlexData-derived Classes**

FlexData-derived classes placed under FlexRecord have restrictions on the placement order depending on their type. From left to right, FlexTreeHeader, FlexGroupHeader, FlexHeader, and other FlexData-derived classes should be in that order.

You cannot display the FlexTreeHeader on the far right or the FlexHeader on the left side of the FlexGroupHeader.

**Constraints Layout of FlexHeader and Derived Classes**
 
FlexHeader and derived classes cannot co-exist with a class that is not derived from FlexHeader, such as FlexLabel, under FlexRowSet or FlexColumnSet. Header columns always occupy one row.

**Constraints Layout of the FlexTreeHeader Class**
 
The FlexTreeHeader class cannot be placed under FlexRowSet. Always occupy one line.

**Constraints in Mobile Version**
 
The Mobile version does not implement FlexRowSet, FlexColumnSet, FlexGroupHeader, FlexTreeHeader, and their corresponding FlexCell.
<br><small><span style="color:red">The above classes are available from Mobile Ver.4.5.0</span></small>


**Restrictions when visual style is enabled**
 
◆ FlexItem.TitleBgColor is disabled because it gives priority to the theme display.<br>
◆ FlexButton.BgColor is disabled because it gives priority to the theme display.


**Precautions when scaling**
 
◆ When FlexView is enlarged to eliminate the error of the internal effective area at the time of enlargement, it is adjusted to a size slightly smaller than the logically calculated value.<br>
◆ FlexCheckButton checkboxes are not subject to scaling.<br>
◆ The width of the drop-down button of FlexListBox is not subject to scaling.<br>
◆ FlexIndentLabel folding buttons are not scaled.