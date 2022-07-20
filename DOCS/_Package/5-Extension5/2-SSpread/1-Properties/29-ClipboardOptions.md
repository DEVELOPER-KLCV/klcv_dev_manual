---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ClipboardOptions Property
nav_order: 29
permalink: /package/extension5/sspread/properties/clipboardoptions
---
# {{ page.title }}

Set whether to include the selected header in the data when copying or pasting the data via the clipboard.

Specify a combination of the following values. The initial value is $ ClipboardOptionsCopyPasteAllHeaders.

| Constant                             | Value | Description                        |
|--------------------------------------|:-----:|------------------------------------|
| $ClipboardOptionsNoHeaders           |   0   | Do not copy and paste both headers |
| $ClipboardOptionsCopyRowHeaders      |   1   | Copy row header                   |
| $ClipboardOptionsPasteRowHeaders     |   2   | Paste row header                  |
| $ClipboardOptionsCopyColumnHeaders   |   4   | Copy column header                 |
| $ClipboardOptionsPasteColumnHeaders  |   8   | Paste column header                |
| $ClipboardOptionsCopyPasteAllHeaders |   15  | Copy and paste both headers        |

If copy of the header been specified, the information in the header is also copied to the clipboard when the copy operation including the header is performed.

If paste header been specified, the information in the header will be overwritten if the paste destination contains the header.

Example of usage <br>
```
/ * Line header only * /
ClipboardOptions = $ ClipboardOptionsCopyRowHeaders + $ ClipboardOptionsPasteRowHeaders;
/ * Column headers only * /
ClipboardOptions = $ ClipboardOptionsCopyColumnHeaders + $ ClipboardOptionsPasteColumnHeaders;
 
/ * The following two are the same * /
ClipboardOptions = $ClipboardOptionsCopyPasteAllHeaders;
ClipboardOptions = $ClipboardOptionsCopyRowHeaders + $ClipboardOptionsPasteRowHeaders +
                   $ClipboardOptionsPasteColumnHeaders + $ClipboardOptionsPasteColumnHeaders;
```

Related Items<br>
<a href="/package/extension5/sspread/properties/autoclipboard">AutoClipBoard</a> property<br>
<a href="/package/extension5/sspread/methods/clipboardcopy">ClipBoardCopy</a>, <a href="/package/extension5/sspread/methods/clipboardcut">ClipBoardCut</a>, <a href="/package/extension5/sspread/methods/clipboardpaste">ClipBoardPaste</a> method

### About copy and paste to header

The characters (A, B, C and 1, 2, 3) displayed in the row header and column header in the initial state are not set as cell values. The value copied to the clipboard as information in the header will be a blank string.

When pasting from the clipboard to the header, even if you paste a blank character string, it will not be blank and will be the standard display (A, B, C or 1, 2, 3).