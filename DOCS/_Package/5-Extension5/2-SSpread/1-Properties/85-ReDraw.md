---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ReDraw Property
nav_order: 85
permalink: /package/extension5/sspread/properties/redraw
---
# {{ page.title }}

Allows or disallows redrawing of the entire SSpread.

Unlike other classes, SSpread is immediately reflected in the display when the properties and methods related to the display are executed.

Therefore, if display-related properties and methods are executed continuously, redrawing will occur each time.

Normally, it is only necessary to be able to display the results of setting various properties, and it is possible to improve the appearance and response by omitting the drawing of the execution process.

Set ReDraw = $FALSE at the beginning of the series of processes for SSpread, and set ReDraw = $TRUE at the end of the series of processes.

Please note that if ReDraw remains $FALSE, no redrawing will be performed and the display will be distorted. 

<small><span style="color:red">Added since Ver.5.0.2</span></small>

Example of usage <br>
```
Function OnTouch(e) {
       SprList.ReDraw = $FALSE;
 
       /* SSpreadにデータをロード */
       var fs = new FileSystem;
       var spfr = fs.Open("data.csv", FileSystem.OPEN_READ);
       SprList.LoadTextFile(spfr, "", ",", "", $LoadTextFileNoHeaders);
       spfr.Close();
               
       SprList.UserColAction = $UserColActionSort;
               
       SprList.BlockMode = $TRUE;
       SprList.Row = 1;
       SprList.Row2 = BodyForm.SprList.MaxRows;*/
       SprList.Row2 = -1;
       SprList.Col = 1;
       SprList.Col2 = 3;
       SprList.CellType = $CellTypeNumber;
       SprList.TypeNumberShowSep = $TRUE;
       SprList.TypeNumberSeparator = ",";
       SprList.BlockMode = $FALSE;
       
       SprList.BlockMode = $TRUE;
       SprList.Row = 1;
       SprList.Row2 = -1;
       SprList.Col = 10;
       SprList.Col2 = 15;
       SprList.CellType = $CellTypeNumber;
       SprList.TypeNumberShowSep = $TRUE;
       SprList.TypeNumberSeparator = ",";
       SprList.BlockMode = $FALSE;
 
       SprList.ReDraw = $TRUE;
}
```
