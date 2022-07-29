---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.IsBlockSelected Property
nav_order: 67
permalink: /package/extension5/sspread/properties/isblockselected
---
# {{ page.title }}

Refers to whether the cell block is selected.

Returns $TRUE if the cell block is selected, $FALSE otherwise.

This property is read-only. The initial value is $FALSE.

The position of the selected cell block can be obtained with the SelBlockCol, SelBlockRow, SelBlockCol2, and SelBlockRow2 properties.

Example of usage<br>
```
Function OnBlockSelected(e) {
    if (IsBlockSelected == $TRUE) {
        print(SelBlockCol, SelBlockRow, SelBlockCol2, SelBlockRow2, "\n");
    }
}
```

Related Items<br>
<a href="/package/extension5/sspread/properties/selblockcol">SelBlockCol</a>, <a href="/package/extension5/sspread/properties/selblockcol2">SelBlockCol2</a>, <a href="/package/extension5/sspread/properties/selblockrow">SelBlockRow</a>, <a href="/package/extension5/sspread/properties/selblockrow2">SelBlockRow2</a> properties