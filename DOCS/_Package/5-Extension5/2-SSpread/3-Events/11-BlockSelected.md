---
layout: default

grand_parent: SSpread Class
parent: Events
has_children: false
title: SSpread.BlockSelected Event
nav_order: 11
permalink: /package/extension5/sspread/events/blockselected
---
# {{ page.title }}

Occurs when the cell block has been selected.

The following child objects are attached to the Event object.

| Type   |       Name      | Description                                |
|--------|:---------------:|--------------------------------------------|
| Number |  **_BlockCol_** | Leftmost column number of cell block       |
| Number |  **_BlockRow_** | Row number at the top of the cell block    |
| Number | **_BlockCol2_** | Rightmost column number of cell block      |
| Number | **_BlockRow2_** | Row number at the bottom of the cell block |

The <a href="/package/extension5/sspread/events/selchange">SelChange</a> event is fired during the cell block selection operation.

Example of usage

```
Function OnBlockSelected(e) {
    BlockMode = $TRUE;
    Col = e.BlockCol;
    Row = e.BlockRow;
    Col2 = e.BlockCol2;
    Row2 = e.BlockRow2;
    BackColor = $RED;
    BlockMode = $FALSE;
}
```

Relatd Item<br>
<a href="/package/extension5/sspread/properties/isblockselected">IsBlockSelected</a>, <a href="/package/extension5/sspread/properties/selblockcol">SelBlockCol</a>,  <a href="/package/extension5/sspread/properties/selblockcol2">SelBlockCol2</a>, <br>,  <a href="/package/extension5/sspread/properties/selblockrow">SelBlockRow</a>,  <a href="/package/extension5/sspread/properties/selblockrow2">SelBlockRow2</a>, <a href="/package/extension5/sspread/properties/selectblockoptions">SelectBlockOptions</a> property <br>
<a href="/package/extension5/sspread/events/selchange">SelChange</a> event 