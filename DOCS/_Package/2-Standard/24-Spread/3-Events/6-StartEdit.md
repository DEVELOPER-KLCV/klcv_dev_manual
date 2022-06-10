---
layout: default

grand_parent: Spread Class
parent: Events
has_children: false
title: Spread.StartEdit Event
nav_order: 6
permalink: /package/standard/spread/events/startedit
---
# {{ page.title }}
<br>

Occurs when the cursor moves to a new cell.

 

The following child objects are attached to the Event object.

|  Type  |    Name   | Description           |
|:------:|:---------:|-----------------------|
| Number | **_row_** | Moved row position    |
| Number | **_col_** | Moved column position |

Normally, in the event handler of the StartEdit event, write the code that prepares the cell for editing by the <a href="/package/standard/spread/events/seteditor">SetEditor</a> method. You can edit cells by using a separately defined TextBox object. The <a href="/package/standard/spread/events/stopedit">StopEdit</a> event, which is paired with the StartEdit event, reflects the input contents in the spreadsheet.

Example
```
Number edit_row;
Number edit_col;
Function OnStartEdit(e) {
    var edit;
    switch (e.col) {
    case 0:
        edit = frmSpreadEdit.ebText;   /* 1列目の編集 */
        break;
    case 1:
        edit = frmSpreadEdit.ebNumber; /* 2列目の編集 */
        break;
    case 2:
        edit = frmSpreadEdit.ebDate;   /* 3列目の編集 */
        break;
    default:
        return;
    }
    edit_row = e.row;          /* 編集を開始した行と列を記録 */
    edit_col = e.col;
    edit.Value= GetCell(r, c); /* 入力値をコピー */
    SetEditor(edit);           /* Spreadに貼り付け */
    edit.Visible = $TRUE;      /* 表示 */
    edit.SetFocus();           /* 入力フォーカスセット */
}
```

Since Biz / Browser events go through the event queue, be sure to use the row and col objects that are passed as child objects of the StartEdit event or <a href="/package/standard/spread/events/stopedit">StopEdit</a> event. In the OnStartEdit, OnStopEdit event handler, if you use the  <a href="/package/standard/spread/properties/value">Value</a> and <a href="/package/standard/spread/properties/columnposition">ColumnPosition</a> properties to get the cursor position, it may be different from the position notified by the event.<br><br>

The StartEdit event is paired with the <a href="/package/standard/spread/events/stopedit">StopEdit</a> event, but there is no guarantee of its order of occurrence. Note that the following events can occur:

```
StartEdit (row = 0, col = 0)
StartEdit (row = 1, col = 0)
StopEdit   (row = 0, col = 0)
StopEdit   (row = 1, col = 0)
```
