---
layout: default

grand_parent: 5. Extension5 Package
parent: SSpread Class

title: Events
nav_order: 3
permalink: /package/extension5/sspread/events

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following methods are defined in the SSpread class.

|Name       | Description   |
|----------	|---------------|
|[Advance](/package/extension5/sspread/events/advance) |Occurs when moving focus in the first or last cell  |
|[AfterColMove](/package/extension5/sspread/events/aftercolmove) |Occurs after moving columns by drag and drop<br><small><span style="color:red">Added since Ver.5.0.2</span></small>  |
|[AfterLeaveCell](/package/extension5/sspread/events/afterleavecell) |Occurs after moving the active cell<br><small><span style="color:red">Added since Ver.5.0.2</span></small>   |
|[AfterLeaveRow](/package/extension5/sspread/events/afterleaverow) |Occurs after moving from the current row to another row<br><small><span style="color:red">Added since Ver.5.0.2</span></small>   |
|[AfterRowMove](/package/extension5/sspread/events/afterrowmove) | Occurs after moving rows by drag and drop<br><small><span style="color:red">Added since Ver.5.0.2</span></small>  |
|[AfterUserSort](/package/extension5/sspread/events/afterusersort) |Occurs after data sorting is complete<br><small><span style="color:red">Added since Ver.5.0.2</span></small>   |
|[BeforeColMove](/package/extension5/sspread/events/beforecolmove) |Occurs when trying to move a column by drag and drop  |
|[BeforeEditMode](/package/extension5/sspread/events/beforeeditmode) | Occurs just before the edit mode starts |
|[BeforeRowMove](/package/extension5/sspread/events/beforerowmove) |Occurs when trying to move a row by drag and drop  |
|[BeforeUserSort](/package/extension5/sspread/events/beforeusersort) | Occurs when sorting data |
|[BlockSelected](/package/extension5/sspread/events/blockselected) |Occurs when you have finished selecting cell blocks  |
|[ButtonClicked](/package/extension5/sspread/events/buttonclicked) | Occurs when a button is clicked in a button or check box cell |
|[Change](/package/extension5/sspread/events/change) | Occurs when changing the value of the active cell |
|[CircularFormula](/package/extension5/sspread/events/circularformula) |Occurs when the formula is a circular reference  |
|[Clicked](/package/extension5/sspread/events/clicked) |Occurs when the left mouse button is pressed on a cell  |
|[ColWidthChange](/package/extension5/sspread/events/colwidthchange) | Occurs when changing the width of a column |
|[ComboCloseUp](/package/extension5/sspread/events/combocloseup) | Occurs when the drop-down list of combo box cells is closed |
|[ComboDropDown](/package/extension5/sspread/events/combodropdown) |Occurs when a drop-down list of combo box cells is opened  |
|[ComboSelChange](/package/extension5/sspread/events/comboselchange) | Occurs when changing the selection of a combo box cell |
|[DoubleClicked](/package/extension5/sspread/events/doubleclicked) | Occurs when the left mouse button is double-clicked on a cell |
|[DragDropBlock](/package/extension5/sspread/events/dragdropblock) |Occurs when a cell block is dragged and dropped to another location  |
|[Dropped](/package/extension5/sspread/events/dropped) | Occurs when dropped by drag and drop |
|[EditChange](/package/extension5/sspread/events/editchange) |  Occurs when the value changes in a cell in input mode|
|[EditError](/package/extension5/sspread/events/editerror) |  Occurs when performing an invalid input operation|
|[EditModeOff](/package/extension5/sspread/events/editmodeoff) |Occurs when the input mode is turned off  |
|[EditModeOn](/package/extension5/sspread/events/editmodeon) | Occurs when the input mode is turned on |
|[EnterRow](/package/extension5/sspread/events/enterrow) | Occurs when moving to a new line and entering input mode |
|[LButtonUp](/package/extension5/sspread/events/lbuttonup) | Occurs when the left mouse button is released on a cell |
|[LeaveCell](/package/extension5/sspread/events/leavecell) | Occurs before moving the active cell |
|[LeaveRow](/package/extension5/sspread/events/leaverow) | Occurs before moving from the current row to another row |
|[RButtonUp](/package/extension5/sspread/events/rbuttonup) |Occurs when the right mouse button is released on a cell  |
|[RClicked](/package/extension5/sspread/events/rclicked) | Occurs when the right mouse button is pressed on a cell |
|[RDoubleClicked](/package/extension5/sspread/events/rdoubleclicked) |Occurs when the right mouse button is double-clicked on a cell  |
|[RowHeightChange](/package/extension5/sspread/events/rowheightchange) |Occurs when changing the height  |
|[SelChange](/package/extension5/sspread/events/selchange) | Occurs when selecting a cell block |
|[TopLeftChange](/package/extension5/sspread/events/topleftchange) |  Occurs when changing the leftmost column or top row displayed|
|[UserFormulaEntered](/package/extension5/sspread/events/userformulaentered) |Occurs when typing a formula in a cell  |