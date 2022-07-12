---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.SelChange Event
nav_order: 35
permalink: /package/extension5/sspread/events/selchange
---
# {{ page.title }}


Occurs when a cell block is selected.

The following child objects are attached to the Event object.

| Type   | Name            | Description                                               |
|--------|-----------------|-----------------------------------------------------------|
| Number |  **_BlockCol_** | Leftmost column number of cell block                      |
| Number |  **_BlockRow_** | Row number at the top of the cell block                   |
| Number | **_BlockCol2_** | Rightmost column number of cell block                     |
| Number | **_BlockRow2_** | Row number at the bottom of the cell block                |
| Number |   **_CurCol_**  | Column number of the cell pointed to by the mouse pointer |
| Number |   **_CurRow_**  | Row number of the cell pointed to by the mouse pointer    |

An event occurs every time the selection is changed by mouse operation or Shift + arrow keys.

Example of usage<br>
```
Function OnSelChange (e) {
    print (strf ("% 1st column to % 2nd column, ", e.BlockCol, e.BlockCol2));
    print (strf ("Selected from% 1st row to % 2nd row ", e.BlockRow, e.BlockRow2), "\ n");
    print (strf (" mouse pointer is at (% 1,% 2) " , e.CurCol, e.CurRow), "\ n");
}
```

Related Items<br>
<a href="/package/extension5/sspread/properties/selectblockoptions">SelectBlockOptions</a> property<br>
<a href="/package/extension5/sspread/events/blockselected">BlockSelected</a> event