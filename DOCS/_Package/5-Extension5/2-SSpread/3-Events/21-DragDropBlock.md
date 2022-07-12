---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.DragDropBlock Event
nav_order: 21
permalink: /package/extension5/sspread/events/dragdropblock
---
# {{ page.title }}

Occurs when a cell block is dragged and dropped to another location.

The following child objects are attached to the Event object.

| Type   |       Name      | Description                                                                                                 |
|--------|:---------------:|-------------------------------------------------------------------------------------------------------------|
| Number |    **_Col_**    | The leftmost column number of the cell block from which you dragged                                         |
| Number |    **_Row_**    | The row number at the top of the cell block from which you dragged                                          |
| Number |    **_Col2_**   | Rightmost column number of the cell block from which you dragged                                            |
| Number |    **_Row2_**   | Row number at the bottom of the cell block from which you drag                                              |
| Number |   **_NewCol_**  | The leftmost column number of the cell block to drop to                                                     |
| Number |   **_NewRow_**  | The row number at the top of the cell block to drop to                                                      |
| Number |  **_NewCol2_**  | Rightmost column number of the cell block to drop to                                                        |
| Number |  **_NewRow2_**  | The row number at the bottom of the cell block to drop to                                                   |
| Number | **_Overwrite_** | 0 if the cell block to drop to has no value, non-zero if there is a value                                   |
| Number |   **_Action_**  | Specify move / copy 1 (copy) if dragged and dropped while holding down the [ Ctrl ] key, 0 (move) otherwise |

To use cell block drag and drop, set the <a href="/package/extension5/sspread/events/allowdragdrop">AllowDragDrop</a> property to $TRUE.

Example of usage<br>
```
Function OnDragDropBlock(e) {
    var srcBlock = strf("%1 to %2 , %3 to %4 ", e.Col , e.Col2 , e.Row, e.Row2);
    var dstBlock = strf("%1 column to %2 column , %3 row to %4 row ", e.NewCol, e.NewCol2, e.NewRow, e.NewRow2);
    
    var actionText;
    if (e.Overwrite == $FALSE) {
        if (e.Action == 1) {
            actionText = " copy ";
        } else {
            actionText = " move ";
        }
    } else {
        if (e.Action == 1) {
            actionText = " Overwrite copy ";
        } else {
            actionText = " Overwrite move ";
        }
    }
    MessageBox (strf (" % 3 from [% 1] to [% 2] " , srcBlock, dstBlock, actionText));
}
```

Related Item <br>
<a href="/package/extension5/sspread/properties/allowdragdrop">AllowDragDrop</a> property