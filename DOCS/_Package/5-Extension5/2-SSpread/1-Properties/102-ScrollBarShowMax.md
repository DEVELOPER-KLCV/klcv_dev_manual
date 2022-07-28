---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ScrollBarShowMax Property
nav_order: 102
permalink: /package/extension5/sspread/properties/scrollbarshowmax
---
# {{ page.title }}

Set the scroll range with the scroll box on the scroll bar.

Specify the following values. The initial value is $TRUE.

| Constant | Description                                                                                                        |
|----------|--------------------------------------------------------------------------------------------------------------------|
| $TRUE    | Scroll to maximum row, maximum column ( <a href="/package/extension5/sspread/properties/maxcols">MaxCols</a>, <a href="/package/extension5/sspread/properties/maxrows">MaxRows</a>, property value)                                          |
| $FALSE   | Scroll down to the row or column where the value is entered (to the value of the <a href="/package/extension5/sspread/properties/datacolcnt">DataColCnt</a>, <a href="/package/extension5/sspread/properties/datarowcnt">DataRowCnt</a> property) |

If $FALSE is specified, dragging the scroll box to the end will scroll to the place where the value is entered. Click the lower and right buttons on the scroll bar to scroll to subsequent rows and columns.

Related Items<br>
<a href="/package/extension5/sspread/properties/datacolcnt">DataColCnt</a>, <a href="/package/extension5/sspread/properties/datarowcnt">DataRowCnt</a>, <a href="/package/extension5/sspread/properties/maxcols">MaxCols</a>, <a href="/package/extension5/sspread/properties/maxrows">MaxRows</a>, <a href="/package/extension5/sspread/properties/scrollbars">ScrollBars</a> properties  