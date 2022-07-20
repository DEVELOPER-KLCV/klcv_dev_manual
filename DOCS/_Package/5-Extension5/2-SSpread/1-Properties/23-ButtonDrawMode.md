---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ButtonDrawMode Property
nav_order: 23
permalink: /package/extension5/sspread/properties/buttondrawmode
---
# {{ page.title }}

Sets the range to display when using command button type or combo box type cells.

Specify a combination of the following values. The initial value is $ButtonDrawModeAlways.

| Constant                     | Value | Description                                   |
|------------------------------|:-----:|-----------------------------------------------|
| $ButtonDrawModeAlways        |   0   | Always displayed                              |
| $ButtonDrawModeCurrentCell   |   1   | Display only in active cell                   |
| $ButtonDrawModeCurrentColumn |   2   | Display only in active columns                |
| $ButtonDrawModeCurrentRow    |   4   | Display only on active rows                   |
| $ButtonDrawModeAlwaysButton  |   8   | Always display buttons in command button cell |
| $ButtonDrawModeAlwaysCombo   |  16   | Always display buttons for combo box cells    |

$ButtonDrawModeAlwaysButton, $ButtonDrawModeAlwaysCombo can be specified in combination with $ButtonDrawModeCurrentCell etc. to partially cancel those effects.

 

The following describes a valid setting example by combination.

| Combination                                                | Value | Description                                                                           |
|------------------------------------------------------------|:-----:|---------------------------------------------------------------------------------------|
| $ButtonDrawModeCurrentColumn + $ButtonDrawModeCurrentRow   |   6   | Show command buttons and combo boxes in either the active column or the active row    |
| $ButtonDrawModeAlwaysButton + $ButtonDrawModeCurrentCell   |   9   | Command buttons are always displayed <br> Hide combo boxes other than the active cell |
| $ButtonDrawModeAlwaysButton + $ButtonDrawModeCurrentColumn |   10  | Command buttons are always displayed <br> Hide combo boxes other than active columns  |
| $ButtonDrawModeAlwaysButton + $ButtonDrawModeCurrentRow    |   12  | Command buttons are always displayed <br> Hide combo boxes other than the active row  |
| $ButtonDrawModeAlwaysCombo + $ButtonDrawModeCurrentCell    |  17   | Combo box is always displayed <br> Hide command buttons other than the active cell    |
| $ButtonDrawModeAlwaysCombo + $ButtonDrawModeCurrentColumn  |   18  | Combo box is always displayed <br> Hide command buttons other than the active column  |
| $ButtonDrawModeAlwaysCombo + $ButtonDrawModeCurrentRow     |   20  | Combo box is always displayed <br> Hide command buttons other than the active row    |

If the OperationMode property specifies a mode that handles spreadsheets row by row (Row, Single, Multi, Extended), command buttons and combo boxes will not be displayed regardless of the specification of this property. For row mode ($OperationModeRow), command buttons and combo boxes are displayed only when the row is in the edit state.

Example of usage
```
ButtonDrawMode = $ButtonDrawModeCurrentRow + $ButtonDrawModeAlwaysCombo;
```

Related Item<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a>, <a href="/package/extension5/sspread/properties/operationmode">OperationMode</a> property.