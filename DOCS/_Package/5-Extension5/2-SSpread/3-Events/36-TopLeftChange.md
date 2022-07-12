---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.TopLeftChange Event
nav_order: 36
permalink: /package/extension5/sspread/events/topleftchange
---
# {{ page.title }}

Occurs when scrolling a spreadsheet with keys or scroll bars and changing the leftmost or top row displayed.

The following child objects are attached to the Event object.

| Type   | Name            | Description                                               |
|--------|-----------------|-----------------------------------------------------------|
| Number |  **_BlockCol_** | Leftmost column number of cell block                      |
| Number |  **_BlockRow_** | Row number at the top of the cell block                   |
| Number | **_BlockCol2_** | Rightmost column number of cell block                     |
| Number | **_BlockRow2_** | Row number at the bottom of the cell block                |
| Number |   **_CurCol_**  | Column number of the cell pointed to by the mouse pointer |
| Number |   **_CurRow_**  | Row number of the cell pointed to by the mouse pointer    |

The event also occurs when setting the <a href="/package/extension5/sspread/properties/leftcol">LectCol</a> and  <a href="/package/extension5/sspread/properties/toprow">TopRow</a> properties.

Example of usage<br<>
```
Function OnTopLeftChange(e) {
    Col = e.OldLeft;
    Row = e.OldTop;
    BackColor = $STD;
    Col = e.NewLeft;
    Row = e.NewTop;
    BackColor = $RED;
}
```

Related Item<br>
<a href="/package/extension5/sspread/properties/leftcol">LeftCol</a>,  <a href="/package/extension5/sspread/properties/toprow">TopRow</a> property