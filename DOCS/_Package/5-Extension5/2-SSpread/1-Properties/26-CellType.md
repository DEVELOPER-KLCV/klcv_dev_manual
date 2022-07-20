---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.CellType Property
nav_order: 26
permalink: /package/extension5/sspread/properties/celltype
---
# {{ page.title }}

Sets the data type of cells in the entire spreadsheet, rows, columns, cells, and cell blocks.

Before setting this property, use the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties, and so on to specify what to do.

Specify the following values. The initial value is $CellTypeEdit for normal cells and $CellTypeStaticText for columns and row header cells.

| Constant            | Value | Description         |
|---------------------|:-----:|---------------------|
| $CellTypeDate       |   0   | Date type           |
| $CellTypeEdit       |   1   | Character type      |
| $CellTypePic        |   4   | Mask type           |
| $CellTypeStaticText |   5   | Label type          |
| $CellTypeTime       |   6   | Time type           |
| $CellTypeButton     |   7   | Command button type |
| $CellTypeComboBox   |   8   | Combo box type      |
| $CellTypePicture    |   9   | Picture type        |
| $CellTypeCheckBox   |   10  | Check box type      |
| $CellTypeCurrency   |   12  | Currency type       |
| $CellTypeNumber     |   13  | Numeric type        |
| $CellTypePercent    |   14  | Percentage type     |
| $CellTypeScientific |   15  | Exponential type    |

Example of usage 
```
Col = 2;
Row = 3;
CellType = $ CellTypeDate;
TypeDateFormat = $ TypeDateFormatGEEMMDD;
 
BlockMode = $ TRUE;
Col = 3;
Row = 3;
Col2 = 5;
Row2 = 5;
CellType = $ CellTypeNumber;
TypeNumberDecPlaces = 0;
BlockMode = $ FALSE;
```

### Related properties for each cell data type

These are the following related properties to make settings that are unique to each cell data type.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-llyw{background-color:#c0c0c0;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-llyw">Date type</th>
    <th class="tg-llyw">Character Type</th>
    <th class="tg-llyw">Mask Type</th>
    <th class="tg-llyw">Label Type</th>
    <th class="tg-llyw">Time Type</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky"> <a href="/package/extension5/sspread/properties/typedatecentury">TypeDateCentury</a> <br><a href="/package/extension5/sspread/properties/typedateformat">TypeDateFormat</a> <br><a href="/package/extension5/sspread/properties/typedatemax">TypeDateMax</a><br><a href="/package/extension5/sspread/properties/typedatemin">TypeDateMin</a><br><a href="/package/extension5/sspread/properties/typedateseparator">TypeDateSeparator</a><br><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipses</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typespin">TypeSpin</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a>
    </td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typeeditcharcase">TypeEditCharCase</a><br><a href="/package/extension5/sspread/properties/typeeditcharset">TypeEditCharSet</a><br><a href="/package/extension5/sspread/properties/typeeditmultiline">TypeEditMultiLine</a><br><a href="/package/extension5/sspread/properties/typeeditpassword">TypeEditPassword</a><br><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipses</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typemaxeditlen">TypeMaxEditLen</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipses</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typepicdefaulttext">TypePicDefaultText</a><br><a href="/package/extension5/sspread/properties/typepicmask">TypePicMask</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipses</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typetextprefix">TypeTextPrefix</a><br><a href="/extension5/sspread/properties/typetextshadow">TypeTextShadow</a><br><a href="/package/extension5/sspread/properties/typetextshadowin">TypeTextShadowIn</a><br><a href="/package/extension5/sspread/properties/typetextwordwrap">TypeTextWordWrap</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky" rowspan="5"><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipses</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typespin">TypeSpin</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typetime24hour">TypeTime24Hour</a><br><a href="/package/extension5/sspread/properties/typetimemax">TypeTimeMax</a><br><a href="/package/extension5/sspread/properties/typetimemin">TypeTimeMin</a><br><a href="/package/extension5/sspread/properties/typetimeseconds">TypeTimeSeconds</a><br><a href="/package/extension5/sspread/properties/typetimeseparator">TypeTimeSeparator</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
  </tr>
  <tr>
    <td class="tg-llyw">Command Button Type</td>
    <td class="tg-llyw">Combo Box Type</td>
    <td class="tg-llyw">Picture Type</td>
    <td class="tg-llyw">Check Box Type</td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typebuttonalign">TypeButtonAlign</a><br><a href="/package/extension5/sspread/properties/typebuttoncolor">TypeButtonColor</a><br><a href="/package/extension5/sspread/properties/typebuttondarkcolor">TypeButtonDarkColor</a><br><a href="/package/extension5/sspread/properties/typebuttonlightcolor">TypeButtonLightColor</a><br><a href="/package/package/extension5/sspread/properties/typebuttonpicture">TypeButtonPicture</a><br><a href="/package/extension5/sspread/properties/typebuttonpicturedown">TypeButtonPictureDown</a><br><a href="/extension5/sspread/properties/typebuttonshadowsize">TypeButtonShadowSize</a><br><a href="/package/extension5/sspread/properties/typebuttontext">TypeButtonText</a><br><a href="/package/extension5/sspread/properties/typebuttontextcolor">TypeButtonTextColor</a><br><a href="/package/extension5/sspread/properties/typebuttontype">TypeButtonType</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typecomboboxautosearch">TypeComboBoxAutoSearch</a><br><a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a><br><a href="/package/extension5/sspread/properties/typecomboboxcursel">TypeComboBoxCurSel</a><br><a href="/package/extension5/sspread/properties/typecomboboxeditable">TypeComboBoxEditable</a><br><a href="/package/extension5/sspread/properties/typecomboboxindex">TypeComboBoxIndex</a><br><a href="/package/extension5/sspread/properties/typecomboboxlist">TypeComboBoxList</a><br><a href="/package/extension5/sspread/properties/typecomboboxmaxdrop">TypeComboBoxMaxDrop</a><br><a href="/package/extension5/sspread/properties/typecomboboxstring">TypeComboBoxString</a><br><a href="/package/extension5/sspread/properties/typecomboboxwidth">TypeComboBoxWidth</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typemaxeditlen">TypeMaxEditLen</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typepictcenter">TypePictCenter</a><br><a href="/package/extension5/sspread/properties/typepictmaintainscale">TypePictMaintainScale</a><br><a href="/package/extension5/sspread/properties/typepictpicture">TypePictPicture</a><br><a href="/package/extension5/sspread/properties/typepictstretch">TypePictStretch</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typecheckcenter">TypeCheckCenter</a><br><a href="/package/extension5/sspread/properties/typecheckpicture">TypeCheckPicture</a><br><a href="/package/extension5/sspread/properties/typechecktext">TypeCheckText</a><br><a href="/package/extension5/sspread/properties/typechecktextalign">TypeCheckTextAlign</a><br><a href="/package/extension5/sspread/properties/typechecktype">TypeCheckType</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
  </tr>
  <tr>
    <td class="tg-llyw">Currency Type</td>
    <td class="tg-llyw">Numeric Type</td>
    <td class="tg-llyw">Percentage Type</td>
    <td class="tg-llyw">Exponential Type</td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typecurrencydecimal">TypeCurrencyDecimal</a><br><a href="/package/extension5/sspread/properties/typecurrencydecplaces">TypeCurrencyDecPlaces</a><br><a href="/package/extension5/sspread/properties/typecurrencyleadingzero">TypeCurrencyLeadingZero</a><br><a href="/package/extension5/sspread/properties/typecurrencymax">TypeCurrencyMax</a><br><a href="/package/extension5/sspread/properties/typecurrencymin">TypeCurrencyMin</a><br><a href="/package/extension5/sspread/properties/typecurrencynegstyle">TypeCurrencyNegStyle</a><br><a href="/package/extension5/sspread/properties/typecurrencymposstyle">TypeCurrencyPosStyle</a><br><a href="/package/extension5/sspread/properties/typecurrencyseparator">TypeCurrencySeparator</a><br><a href="/package/extension5/sspread/properties/typecurrencyshowsep">TypeCurrencyShowSep</a><br><a href="/package/extension5/sspread/properties/typecurrencyshowsymbol">TypeCurrencyShowSymbol</a><br><a href="/package/extension5/sspread/properties/typecurrencysymbol">TypeCurrencySymbol</a><br><a href="/package/extension5/sspread/properties/typecurrencyellipses">TypeCurrencyEllipses</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a><br><a href="/package/extension5/sspread/properties/typespin">TypeSpin</a><br><a href="/package/extension5/sspread/properties/typesyncinc">TypeSpinInc</a><br><a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipse</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a><br><a href="/package/extension5/sspread/properties/typenumberdecimal">TypeNumberDecimal</a><br><a href="/package/extension5/sspread/properties/typenumberdecplaces">TypeNumberDecPlaces</a><br><a href="/package/extension5/sspread/properties/typenumberleadingzero">TypeNumberLeadingZero</a><br><a href="/package/extension5/sspread/properties/typenumbermax">TypeNumberMax</a><br><a href="/package/extension5/sspread/properties/typenumbermin">TypeNumberMin</a><br><a href="/package/extension5/sspread/properties/typenumbernegstyle">TypeNumberNegStyle</a><br><a href="/package/extension5/sspread/properties/typenumberseparator">TypeNumberSeparator</a><br><a href="/package/extension5/sspread/properties/typenumbershowsep">TypeNumberShowSep</a><br><a href="/package/extension5/sspread/properties/typespin">TypeSpin</a><br><a href="/package/extension5/sspread/properties/typesyncinc">TypeSpinInc</a><br><a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipse</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a><br><a href="/package/extension5/sspread/properties/typepercentdecimal">TypePercentDecimal</a><br><a href="/package/extension5/sspread/properties/typepercentdecplaces">TypePercentDecPlaces</a><br><a href="/package/extension5/sspread/properties/typepercentdecimal">TypePercentDecimal</a><br><a href="/package/extension5/sspread/properties/typepercentleadingzero">TypePercentLeadingZero</a><br><a href="/package/extension5/sspread/properties/typepercentmax">TypePercentMax</a><br><a href="/package/extension5/sspread/properties/typepercentmin">TypePercentMin</a><br><a href="/package/extension5/sspread/properties/typepercentnegstyle">TypePercentNegStyle</a><br><a href="/package/extension5/sspread/properties/typespin">TypeSpin</a><br><a href="/package/extension5/sspread/properties/typesyncinc">TypeSpinInc</a><br><a href="/package/extension5/sspread/properties/typespinwrap">TypeSpinWrap</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
    <td class="tg-0pky"><a href="/package/extension5/sspread/properties/typeellipses">TypeEllipse</a><br><a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a><br><a href="/package/extension5/sspread/properties/typenegred">TypeNegRed</a><br><a href="/package/extension5/sspread/properties/typescientificdecimal">TypeScientificDecimal</a><br><a href="/package/extension5/sspread/properties/typescientificdecplaces">TypeScientificDecPlaces</a><br><a href="/package/extension5/sspread/properties/typescientificmax">TypeScientificMax</a><br><a href="/package/extension5/sspread/properties/typescientificmin">TypeScientificMin</a><br><a href="/package/extension5/sspread/properties/typetextorient">TypeTextOrient</a><br><a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a></td>
  </tr>
</tbody>
</table>

### Property inheritance for each cell data type

For related properties whose names start with "Type", the last setting for each cell data type is remembered, and the property is inherited the next time the property is set for a cell with the same data type.

For example, if set the <a href="/package/extension5/sspread/properties/typedatemax">TypeDateMax</a> property or <a href="/package/extension5/sspread/properties/typedatemin">TypeDateMin</a> property after setting the date type ($CellTypeDate), the same settings will be inherited for the date type cells created after that.

Initial values for related properties are stored for each cell data type. The <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a> property, <a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> property, etc. used for multiple data types are also managed separately for each data type.

The stored settings will be applied together when setting the data type of subsequent cells. This feature is useful if have the same settings for multiple cells, but be careful if it have different settings.

・ Operation Image

(1) The value of the related property is held for each data type.

<a href="/img/package/ext5-sspread-celltype1.PNG" target="_blank">
<img src="/img/package/ext5-sspread-celltype1.PNG" alt="login image">
</a>

(2) When setting the CellType property, set all the contents of (1) corresponding to the set data type at the same time.

```
CellType = $CellTypeDate;
```

<a href="/img/package/ext5-sspread-celltype2.PNG" target="_blank">
<img src="/img/package/ext5-sspread-celltype2.PNG" alt="login image">
</a>

(3) When setting related properties that start with "Type", set all the contents of (1) at the same time after updating (1).

```
TypeDateMin = "19500101";
```

<a href="/img/package/ext5-sspread-celltype3.PNG" target="_blank">
<img src="/img/package/ext5-sspread-celltype3.PNG" alt="login image">
</a>

Program Example

```
Col = 1; / * Set column 1 row 1 cell * /
Row = 1;
CellType = $ CellTypeDate;     / * Set to date type * /
TypeDateMin = "19500101";     / * Set the start of the date range to 1950/01/01 * /
TypeDateMax = "20501231";     / * Set end of date range to 2050/12/31 * /
print (Col, Row, TypeDateMin, TypeDateMax, "\ n");
 
Col = 2; / * Set column 2 rows 2 cells * /
Row = 2;
CellType = $ CellTypeDate;     / * Set to date type (date range is also the same as 1 row 1 cell in column (1950/01/01 ~ 2050/12/31) ) * /
print (Col, Row, TypeDateMin, TypeDateMax, "\ n");
 
Col = 3; / * Set column 3 rows 3 cells * /
Row = 3;
CellType = $ CellTypeDate;     / * Set to date type (at this point the date range is the same as column 1 row 1 and column 2 row 2 cells) * /
TypeDateMin = "20000101";     / * Set the start of the date range to 2000/01/01 (date range will be from 2000/01/01 to 2050/12/31 ) * /
print (Col, Row, TypeDateMin, TypeDateMax, "\ n");
 
Col = 4; / * Change column 4 rows 4 cells * /
Row = 4;
CellType = $ CellTypeDate;     / * Set to date type (date range is the same as column 3 rows 3 cells ( 2000/01/01 ~ 2050/12/31) ) * /
print (Col, Row, TypeDateMin, TypeDateMax, "\ n");
 
/ * Setting example that requires attention * /
Col = 1; / * Change column 1 row 1 cell again * /
Row = 1;
/ * At this point, as originally set (1950/01/01 ~ 2050/12/31) * /
print (Col, Row, TypeDateMin, TypeDateMax, "\ n");
 
TypeDateMax = "20001231";     / * Since the previous date type setting (column 4 row 4 cell setting) is the default value, all the original settings are overwritten * /
                             / * As a result, the value of TypeDateMin is also changed, and the date range is from 2000/01/01 to 2000/12/31 * /
print (Col, Row, TypeDateMin, TypeDateMax, "\ n");
```

### Notes on property inheritance when applying to cell blocks

When <a href="/package/extension5/sspread/properties/blockmode">BlockMode</a> is set to $TRUE and the setting is applied to the cell block, each property is set based on the cell pointed to by the <a href="/package/extension5/sspread/properties/col">Col</a>, <a href="/package/extension5/sspread/properties/row">Row</a> properties.

For example, if the cell pointed to by the Col and Row properties is a combo box cell, all cells in the cell block will be changed to combo box cells and the same settings will be applied.

Please take note that changing the <a href="/package/extension5/sspread/properties/typehalign">TypeHAlign</a>, <a href="/package/extension5/sspread/properties/typevalign">TypeVAlign</a> properties, etc., which are common to many data types, will result in the same settings, including the cell data type.

### Notes on property inheritance of combo box type cells

In the combo box type cell, the following properties and methods that operate on list items are not subject to property inheritance.

<a href="/package/extension5/sspread/properties/typecomboboxcursel">TypeComboBoxCurSel</a> property<br><a href="/package/extension5/sspread/properties/typecomboboxlist">TypeComboBoxList</a> property<br><a href="/package/extension5/sspread/properties/typecomboboxstring">TypeComboBoxString</a> property<br><a href="/package/extension5/sspread/methods/typecomboboxclear">TypeComboBoxClear</a> method<br><a href="/package/extension5/sspread/methods/typecomboboxremoveitem">TypeComboBoxRemoveItem</a> method<br>
Working with list items using these does not affect the setting of the CellType property or the related properties of combo box cells that start with "Type".

The <a href="/package/extension5/sspread/properties/typecomboboxcount">TypeComboBoxCount</a> property is read-only and is not subject to property inheritance.

The <a href="/package/extension5/sspread/properties/typecomboboxindex">TypeComboBoxIndex</a> property only acts as a variable, so it holds only one value, regardless of the state of the cell.

### Notes on property inheritance of label type cells

Label type cells hold data for property inheritance separately because the initial values are different between normal cells, column header cells, and row header cells.

<a href="/img/package/ext5-sspread-celltype4.PNG" target="_blank">
<img src="/img/package/ext5-sspread-celltype4.PNG" alt="login image">
</a>

Settings for related properties of labeled cells that start with "Type" will update both of these data. Each data is used for the setting to the cell.

```
TypeHAlign = $ TypeHAlignRight;
```

<a href="/img/package/ext5-sspread-celltype5.PNG" target="_blank">
<img src="/img/package/ext5-sspread-celltype5.PNG" alt="login image">
</a>

### About display of command button type and combo box type cells

In command button type and combo box type cells, command buttons and combo boxes are usually always displayed, but you can control the display / non-display by the position of the active cell by setting the <a href="/package/extension5/sspread/properties/buttondrawmode">ButtonDrawMode</a>  property.

If the <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a>  property specifies a mode that handles spreadsheets row by row (Row, Single, Multi, Extended), the command buttons and combo boxes will not be displayed. For row mode ($OperationModeRow), command buttons and combo boxes are displayed only when the row is in the edit state.

In read-only mode ($OperationModeRead), command buttons and combo boxes are displayed but not available.
For command button type and combo box type cells, use in standard mode ($OperationModeNormal) or row mode ($OperationModeRow).