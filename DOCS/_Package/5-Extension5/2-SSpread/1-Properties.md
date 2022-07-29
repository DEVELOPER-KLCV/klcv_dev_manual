---
layout: default

grand_parent: 5. Extension5 Package
parent: SSpread Class

title: Properties
nav_order: 1
permalink: /package/extension5/sspread/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the SSpread class.

|Name       | Access | [&=]() | Type   | Initial Value | Description   |
|----------	|--------|--------|--------|---------------|---------|
|[AcceptDrop](/package/extension5/sspread/properties/acceptdrop) | CRW | | integer | 0 | Type that accepts drag and drop |
|[ActiveCellHighlightStyle](/package/extension5/sspread/properties/activecellhighlightstyle) | CRW | | integer | $ActiveCellHighlightStyleNormal | Highlight active cell |
| [ActiveCol](/package/extension5/sspread/properties/activecol) | R | | integer | 1 | Active cell column number |
| [ActiveRow](/package/extension5/sspread/properties/activerow) | R | | integer | 1 | Active cell row number |
| [AllowCellOverflow](/package/extension5/sspread/properties/allowcelloverflow) | CRW | | boolean | $FALSE |Displayed in the next cell |
| [AllowColMove](/package/extension5/sspread/properties/allowcolmove) | CRW | | boolean |$FALSE | Allow drag and drop to move columns |
| [AllowDragDrop](/package/extension5/sspread/properties/allowdragdrop) | CRW | | boolean | $FALSE | Allow drag and drop of cell blocks |
| [AllowEditOverflow](/package/extension5/sspread/properties/alloweditoverflow) | CRW | | boolean | $FALSE | In the input mode, it is displayed so that it extends beyond the adjacent cell. |
| [AllowMultiBlocks](/package/extension5/sspread/properties/allowmultiblocks) | CRW | | boolean | $FALSE | Allow multiple selection of cell blocks |
| [AllowRowMove](/package/extension5/sspread/properties/allowrowmove) | CRW || boolean | $FALSE | Allow drag and drop to move rows |
|[AllowUserFormulas](/package/extension5/sspread/properties/allowuserformulas) | CRW | | boolean | $FALSE | Allow entry of formulas |
|[Appearance](/package/extension5/sspread/properties/appearance) | CRW || integer | $AppearanceFlat | Borders across the spreadsheet |
| [AppearanceStyle](/package/extension5/sspread/properties/appearancestyle) | CRW | | integer | $AppearanceStyleEnhanced | Overall spreadsheet design |
|[ArrowsExitEditMode](/package/extension5/sspread/properties/arrowsexiteditmode) | CRW | | boolean | $FALSE | Operation of arrow keys in input mode |
|[AutoCalc](/package/extension5/sspread/properties/autocalc) | CRW || boolean | $TRUE | Automatically recalculate each formula in related cells |
|[AutoClipboard](/package/extension5/sspread/properties/autoclipboard) | CRW || boolean | $TRUE | Enable shortcut keys to operate the clipboard |
|[BackColor](/package/extension5/sspread/properties/backcolor) | CRW | × | integer<br>UString | $WHITE | Background color for rows, columns, cells, cell blocks |
|[BackColorStyle](/package/extension5/sspread/properties/backcolorstyle) |CRW | |integer | $BackColorStyleOverGrid | Display background color above grid lines |
|[BgColor](/package/extension5/sspread/properties/bgcolor) | CRW | × | integer<br>UString | $WHITE | Background color for rows, columns, cells, cell blocks |
|[BlockMode](/package/extension5/sspread/properties/blockmode) | CRW | × | boolean | $FALSE | Enable the value of each property for the cell block |
|[Border](/package/extension5/sspread/properties/border) | CRW || boolean | $FALSE | Display of border |
|[BorderStyle](/package/extension5/sspread/properties/borderstyle) | CRW | × | boolean | $FALSE | Display of border |
|[ButtonDrawMode](/package/extension5/sspread/properties/buttondrawmode)| CRW | | integer | $ButtonDrawModeAlways |  Button type, combo box type cell button display range|
|[CellNote](/package/extension5/sspread/properties/cellnote) | CRW | × | UString | "" | Cell comment settings<br>**<small>Added since Version 5.0.2</small>** |
| [CellTag](/package/extension5/sspread/properties/celltag) | CRW | × | UString | "" | User-defined tags for cells, columns and rows |
|[CellType](/package/extension5/sspread/properties/celltype) | CRW | × | integer | $CellTypeEdit | Data types of cells in rows, columns, cells, cell blocks |
|[ChangeMade](/package/extension5/sspread/properties/changemade) | CRW | × | boolean | $FALSE | Whether the cell value has changed |
|[Clip](/package/extension5/sspread/properties/clip) | CRW | × | UString | - | Set the value in the cell block |
|[ClipboardOptions](/package/extension5/sspread/properties/clipboardoptions) | CRW | | integer | $ClipboardOptionsCopyPasteAllHeaders | Handling of headers when copying and pasting |
|[ClipValue](/package/extension5/sspread/properties/clipvalue) | CRW | × | UString | - | Set the value in the cell block |
|[Col](/package/extension5/sspread/properties/col) | CRW | × | integer | -1 | Columns to be processed |
|[Col2](/package/extension5/sspread/properties/col2) | CRW | × | integer | 0 | The last column of the cell block to be processed |
|[ColHeadersAutoText](/package/extension5/sspread/properties/colheadersautotext)| CRW| | integer| $DispLetters| Display format of column header |
|[ColHeadersShow](/package/extension5/sspread/properties/colheadersshow)| CRW| | boolean| $TRUE| Show / hide column headers |
|[ColHidden](/package/extension5/sspread/properties/colhidden)| CRW| ×| boolean| $FALSE| Show / hide columns |
|[ColID](/package/extension5/sspread/properties/colid)| CRW| ×| UString| ""| A string that identifies the column |
|[ColMerge](/package/extension5/sspread/properties/colmerge)| CRW| ×| integer| $MergeNone| Group cells with the same content in a particular column |
|[ColsFrozen](/package/extension5/sspread/properties/colsfrozen)| CRW| | integer| 0| Number of columns to be fixedly displayed without scrolling |
|[ColUserSortIndicator](/package/extension5/sspread/properties/colusersortindicator)| ※| ×| integer| $ColUserSortIndicatorNone| Show / hide sort indicator | 
|[ColWidth](/package/extension5/sspread/properties/colwidth)| ※| ×| integer| 64| Column width |
|[CursorIcon](/package/extension5/sspread/properties/cursoricon)| CRW| ×| String<br>Object Reference| -| User-defined mouse cursor |
|[CursorStyle](/package/extension5/sspread/properties/cursorstyle)| CRW| ×| integer| $CursorStyleDefault| Mouse cursor shape to use |
|[CursorType](/package/extension5/sspread/properties/cursortype)| CRW| ×| integer| $CursorTypeDefault| Target to set the mouse cursor |
|[DataColCnt](/package/extension5/sspread/properties/datacolcnt)| R| | integer| 0| Column number of the last cell where the value is entered |
|[DataRowCnt](/package/extension5/sspread/properties/datarowcnt)| R| |integer| 0| Row number of the last cell where the value is entered |
|[EditEnterAction](/package/extension5/sspread/properties/editenteraction)| CRW| | integer| $EditEnterActionNone| Enter key behavior | 
|[EditMode](/package/extension5/sspread/properties/editmode)| CRW| ×| boolean| $FALSE| Input mode status | 
|[EditModePermanent](/package/extension5/sspread/properties/editmodepermanent)| CRW| | boolean| $FALSE| Input mode is always ON |
|[EditModeReplace](/package/extension5/sspread/properties/editmodereplace)| CRW| | boolean| $FALSE | Replace with original value in input mode |
|[FgColor](/package/extension5/sspread/properties/fgcolor)| CRW| ×| integer<br>UString| $BLACK| Text color of rows, columns, cells, cell blocks |
|[FontBold](/package/extension5/sspread/properties/fontbold)| CRW| ×| boolean| $FALSE| Bold font for rows, columns, cells, and cell blocks|
|[FontFace](/package/extension5/sspread/properties/fontface)| CRW| ×| integer| $STD| Row, column, cell, cell block font styles |
|[FontItalic](/package/extension5/sspread/properties/fontitalic)| CRW| ×| boolean| $FALSE| Font italics for rows, columns, cells and cell blocks|
|[FontKind](/package/extension5/sspread/properties/fontkind)| CRW| ×| integer<br>UString| $STD| Row, column, cell, cell block font types |
|[FontName](/package/extension5/sspread/properties/fontname) |CRW| ×| UString | "ＭＳ ＰGothic"| Font names for rows, columns, cells, and cell blocks |
|[FontSize](/package/extension5/sspread/properties/fontsize)| CRW| ×| integer| 10| Row, column, cell, cell block font size |
|[FontStrikethru](/package/extension5/sspread/properties/fontstrikethru)| CRW| ×| boolean| $FALSE| Font strikethrough for rows, columns, cells, and cell blocks |
|[FontUnderline](/package/extension5/sspread/properties/fontunderline)| CRW| ×| boolean| $FALSE| Underline fonts for rows, columns, cells, and cell blocks |
|[ForeColor](/package/extension5/sspread/properties/forecolor)| CRW| ×| integer<br>UString| $BLACK| Text color of rows, columns, cells, cell blocks |
|[Formula](/package/extension5/sspread/properties/formula)| CRW| ×| UString| "" | Cell formula |
|[FormulaSync](/package/extension5/sspread/properties/formulasync)| CRW| | boolean| $TRUE| Automatically update cell references in formulas |
|[GrayAreaBackColor](/package/extension5/sspread/properties/grayareabackcolor)| CRW| | integer<br>UString| $STD| Background color of gray area |
|[GridColor](/package/extension5/sspread/properties/gridcolor) | CRW| | integer<br>UString| $STD| Display color of grid lines |
|[GridShowHoriz](/package/extension5/sspread/properties/gridshowhoriz)| CRW| | boolean| $TRUE| Show / hide horizontal grid lines |
|[GridShowVert](/package/extension5/sspread/properties/gridshowvert)| CRW| | boolean| $TRUE| Show / hide vertical grid lines| 
|[GridSolid](/package/extension5/sspread/properties/gridsollid)| CRW | | boolean| $TRUE| Grid line type |
|[IsBlockSelected](/package/extension5/sspread/properties/isblockselected)| R| | boolean| $FALSE| Whether cell block is selected |
|[LeftCol](/package/extension5/sspread/properties/leftcol)| CRW| | integer| 1| Column number to display in the leftmost column |
|[Lock](/package/extension5/sspread/properties/lock)| CRW| ×| boolean| $FALSE| Lock rows, columns, cells, cell blocks|
|[LockBackColor](/package/extension5/sspread/properties/lockbackcolor)| CRW| | integer<br>UString| $STD| Background color of locked cells |
|[LockForeColor](/package/extension5/sspread/properties/lockforecolor)| CRW| | integer<br>UString| $STD| Text color of locked cell |
|[MaxCols](/package/extension5/sspread/properties/maxcols)| CRW| | integer| 500| Total number of columns |
|[MaxRows](/package/extension5/sspread/properties/maxrows)| CRW| | integer| 500| Total number of rows |
|[MaxTextCellHeight](/package/extension5/sspread/properties/maxtextcellheight)| R| ×| integer| -| Height required to display the text set in the cell |
|[MaxTextCellWidth](/package/extension5/sspread/properties/maxtextcellwidth)| R| ×| integer| -| The width required to display the text set in the cell |
|[MaxTextColWidth](/package/extension5/sspread/properties/maxtextcolwidth)| ※| × | integer | - | The width required to display the text set in the column |
|[MaxTextRowHeight](/package/extension5/sspread/properties/maxtextrowheight)| ※| ×| integer| -| The height required to display the text set on the line |
|[MoveActiveOnFocus](/package/extension5/sspread/properties/moveactiveonfocus)| CRW| | boolean| $TRUE| Activates the cell pointed to by the mouse pointer when getting focus |
|[NoBeep](/package/extension5/sspread/properties/nobeep)| CRW| | boolean| $FALSE| Beep when you make a mistake or make a mistake |
|[NoBorder](/package/extension5/sspread/properties/noborder)| CRW| | boolean| $FALSE| Show / Hide Borders at Right and Bottom Edges of Spreadsheets |
|[OperationMode](/package/extension5/sspread/properties/operationmode)| CRW| | integer| $OperationModeNormal| Operation mode |
|[ProcessDelete](/package/extension5/sspread/properties/processdelete)| CRW| | Integer| $DeleteNone| Delete the data and formula in the selected cell with the Delete key.<br>**<small>Added since Version 5.0.2</small>** |
|[ProcessTab](/package/extension5/sspread/properties/processtab)| CRW| | boolean| $FALSE| Move the active cell with the Tab key |
|[Protect](/package/extension5/sspread/properties/protect)| CRW|  | boolean| $TRUE| Prohibit writing of locked cells |
|[ReDraw](/package/extension5/sspread/properties/redraw)| CRW| | boolean| $TRUE| Allow redraw<br>**<small>Added since Version 5.0.2</small>** |
|[RestrictCols](/package/extension5/sspread/properties/restrictcols)| CRW| | boolean| $FALSE| Prohibit entering a value if no value has been entered in the column to the left |
|[RestrictRows](/package/extension5/sspread/properties/restrictrows)| CRW| | boolean| $FALSE| Prohibit entering a value if no value has been entered in the next line above |
|[RetainSelBlock](/package/extension5/sspread/properties/retainselblock)| CRW| | boolean| $FALSE| Leave selection highlighted when out of focus |
|[Row](/package/extension5/sspread/properties/row)| CRW| ×| integer| -1| Line to be processed |
|[Row2](/package/extension5/sspread/properties/row2)| CRW| ×| integer| 0| The last row of the cell block to be processed |
|[RowHeadersAutoText](/package/extension5/sspread/properties/rowheadersautotext)| CRW| | integer| $DispNumbers| Line header display format |
|[RowHeadersShow](/package/extension5/sspread/properties/rowheadersshow)| CRW| | boolean| $TRUE| Show / hide line headers |
|[RowHeight](/package/extension5/sspread/properties/rowheight)| ※| ×| integer| 15| Row height |
|[RowHidden](/package/extension5/sspread/properties/rowhidden)| CRW| ×| boolean| $FALSE| Show / hide rows |
|[RowMerge](/package/extension5/sspread/properties/rowmerge)| CRW| ×| integer| $MergeNone| Group cells with the same content within a particular row |
|[RowsFrozen](/package/extension5/sspread/properties/rowsfrozen)| CRW| | integer| 0| Number of lines to be fixedly displayed without scrolling |
|[ScrollBarExtMode](/package/extension5/sspread/properties/scrollbarextmode)| CRW| | boolean| $FALSE| Automatically show / hide scrollbars |
|[ScrollBarHColor](/package/extension5/sspread/properties/scrollbarhcolor) | CRW| | integer<br>UString| $STD| Horizontal scrollbar color |
|[ScrollBarHeight](/package/extension5/sspread/properties/scrollbarheight)| CRW| | integer| -1| Horizontal scroll bar height |
|[ScrollBarMaxAlign](/package/extension5/sspread/properties/scrollbarmaxalign)| CRW| | boolean| $TRUE| Display position of the last cell when scrolling to the end |
|[ScrollBars](/package/extension5/sspread/properties/scrollbars)| CRW| | integer| $ScrollBarsBoth| Show / hide scrollbar|
|[ScrollBarShowMax](/package/extension5/sspread/properties/scrollbarshowmax)| CRW| | boolean| $TRUE| Scroll range (until the last data, up to the last cell) |
|[ScrollBarStyle](/package/extension5/sspread/properties/scrollbarstyle)| CRW| | integer| $ScrollBarStyleInherit| Scroll bar design |
|[ScrollBarTrack](/package/extension5/sspread/properties/scrollbartrack)| CRW| | integer| $ScrollBarTrackOff| Show spreadsheet contents while scrolling| 
|[ScrollBarVColor](/package/extension5/sspread/properties/scrollbarvcolor)| CRW| | integer<br>UString| $STD| Vertical scrollbar color |
|[ScrollBarWidth](/package/extension5/sspread/properties/scrollbarwidth)| CRW| | integer| -1| Vertical scrollbar width |
|[SelBackColor](/package/extension5/sspread/properties/selbackcolor)| CRW| | integer<br>UString| $STD| Background color of the selected cell or cell block |
|[SelBlockCol](/package/extension5/sspread/properties/selblockcol)|R| | integer| 0| Leftmost column number of the selected cell block |
|[SelBlockCol2](/package/extension5/sspread/properties/selblockcol2)| R|  | integer| 0| Rightmost column number of the selected cell block |
|[SelBlockRow](/package/extension5/sspread/properties/selblockrow)| R| | integer| 0| Row number at the top of the selected cell block| 
|[SelBlockRow2](/package/extension5/sspread/properties/selblockrow2)| R| | integer| 0| Row number at the bottom of the selected cell block |
|[SelectBlockOptions](/package/extension5/sspread/properties/selectblockoptions)| CRW| ×| integer| 15| Options when selecting cell blocks |
|[SelectionCount](/package/extension5/sspread/properties/selectioncount)| R| |integer| 0| Number of selected cell blocks or number of rows when multiple rows are selected |
|[SelForeColor](/package/extension5/sspread/properties/selforecolor)| CRW| | integer<br>UString| $STD| Text color of the selected cell or cell block |
|[SelLength](/package/extension5/sspread/properties/sellength)| CRW| ×| integer| -| Number of characters for character selection in input mode |
|[SelModeIndex](/package/extension5/sspread/properties/selmodeindex)| CRW| ×| integer| -| Line number to select in single selection mode |
|[SelModeSelected](/package/extension5/sspread/properties/selmodeselected)| CRW| ×| boolean| - | Select the row indicated by the Row property in multiple selection mode |
|[SelStart](/package/extension5/sspread/properties/selstart)| CRW| ×| integer| -| Start position of character selection in input mode |
|[SelText](/package/extension5/sspread/properties/seltext)| CRW| ×| UString| -| Character string for character selection in input mode|
|[ShadowColor](/package/extension5/sspread/properties/shadowcolor)| CRW| | integer<br>UString| $STD| Row and column headers, and label cell background color |
|[ShadowDark](/package/extension5/sspread/properties/shadowdark)| CRW| | integer<br>UStrig| $STD| Row and column headers, and the color of the shadow side of the unevenness of the label type cell |
|[ShadowLight](/package/extension5/sspread/properties/shadowlight)| CRW| | integer<br>UString| $STD| Light side color of row and column headers and unevenness of label type cells<br>**<small>Added since Version 5.0.1</small>** |
|[ShadowText](/package/extension5/sspread/properties/shadowtext)| CRW| | integer<br>UString| $STD| Text color for row and column headers and label cells |
|[SortKey](/package/extension5/sspread/properties/sortkey)| ※| ×| integer| -| Sort key|
|[SortKeyOrder](/package/extension5/sspread/properties/sortkeyorder)| ※| ×| integer| $SortKeyOrderAscending| Sort order| 
|[StartingColNumber](/package/extension5/sspread/properties/startingcolnumber)| CRW| | integer| 1| Column display start number |
|[StartingRowNumber](/package/extension5/sspread/properties/startingrownumber)| CRW| | integer| 1| Line display start number |
|[Text](/package/extension5/sspread/properties/text)| CRW| ×| UString| ""| Cell value| 
|[ToolTip](/package/extension5/sspread/properties/tooltip)| CRW| | String| ""| Value to display in tooltip |
|[ToolTipDelayTime](/package/extension5/sspread/properties/tooltipdelaytime)| CRW| | integer| 0| Time to display tooltips |
|[TopRow](/package/extension5/sspread/properties/toprow)| CRW| | integer| 1 | The number of the line to be displayed on the top line |
|[TwoDigitYearMax](/package/extension5/sspread/properties/twodigityearmax)| CRW| | integer | 2059| Base year for converting a 2-digit year to a 4-digit year|
|[TypeButtonAlign](/package/extension5/sspread/properties/typebuttonalign)| CRW| ×| integer| $TypeButtonAlignBottom| Arrangement of characters in button cell |
|[TypeButtonColor](/package/extension5/sspread/properties/typebuttoncolor)| CRW| ×| integer<br>UString| (OS settings)| Button cell background color |
|[TypeButtonDarkColor](/package/extension5/sspread/properties/typebuttondarkcolor)| CRW| ×| integer<br>UString| (OS settings) | The color of the shadow side of the unevenness of the button cell |
|[TypeButtonLightColor](/package/extension5/sspread/properties/typebuttonlightcolor)| CRW| ×| integer<br>UString| (OS settings)| The color of the unevenness of the button cell on the light side| 
|[TypeButtonPicture](/package/extension5/sspread/properties/typebuttonpicture)| CRW| ×| String<br>Object Reference| -| Image of button cell not pressed |
|[TypeButtonPictureDown](/package/extension5/sspread/properties/typebuttonpicturedown)| CRW| ×| String<br>Object Reference| -| Image of the pressed state of the button cell |
|[TypeButtonShadowSize](/package/extension5/sspread/properties/typebuttonshadowsize)| CRW| ×| integer| 1| Depth of unevenness of button cell |
|[TypeButtonText](/package/extension5/sspread/properties/typebuttontext)| CRW| ×|  UString| ""| Button cell text|
|[TypeButtonTextColor](/package/extension5/sspread/properties/typebuttontextcolor)| CRW| ×| integer<br>UString| (OS settings)| Text color of button cell |
|[TypeButtonType](/package/extension5/sspread/properties/typebuttontype)| CRW| ×| integer| $TypeButtonTypeNormal| Button type of button cell |
|[TypeCheckCenter](/package/extension5/sspread/properties/typecheckcenter)| CRW| ×| boolean| $FALSE|Check box type cell check box is placed in the center |
|[TypeCheckPicture](/package/extension5/sspread/properties/typecheckpicture)| ※ | × | String<br>Object Reference| -| Check box image of check box type cell |
|[TypeCheckText](/package/extension5/sspread/properties/typechecktext)| CRW | ×| UString| "" | Checkbox cell text |
|[TypeCheckTextAlign](/package/extension5/sspread/properties/typechecktextalign)| CRW| ×| integer| $TypeCheckTextAlignRight| Arrangement of characters in check box type cells |
|[TypeCheckType](/package/extension5/sspread/properties/typechecktype)| CRW| ×| integer| $TypeCheckTypeNormal| Check box type of check box type cell |
|[TypeComboBoxAutoSearch](/package/extension5/sspread/properties/typecomboboxautosearch)| CRW| ×| integer| $TypeComboBoxAutoSearchSingleChar| Combo box cell search type |
|[TypeComboBoxCount](/package/extension5/sspread/properties/typecomboboxcount)| R| ×| integer| 0| Number of items in combo box type cell |
|[TypeComboBoxCurSel](/package/extension5/sspread/properties/typecomboboxcursel)| CRW| ×| integer| -1| Selected item number of combo box type cell|
|[TypeComboBoxEditable](/package/extension5/sspread/properties/typecomboboxeditable)| CRW| ×| boolean| $FALSE| Make the item name of the combo box type cell editable |
|[TypeComboBoxIndex](/package/extension5/sspread/properties/typecomboboxindex)| CRW| ×| integer| 0| Item number to be processed by combo box type cell| 
|[TypeComboBoxList](/package/extension5/sspread/properties/typecomboboxlist)| CRW| ×| UString| "" | List of item names for combo box cell |
|[TypeComboBoxMaxDrop](/package/extension5/sspread/properties/typecomboboxmaxdrop)| CRW| ×| integer| 6| Number of rows to display in the drop-down list of combo box cells |
|[TypeComboBoxString](/package/extension5/sspread/properties/typecomboboxstring)| CRW| ×| UString| -| Item name of combo box type cell |
|[TypeComboBoxWidth](/package/extension5/sspread/properties/typecomboboxwidth)| CRW| ×| integer| 0| Combo box cell drop-down list width | 
|[TypeCurrencyDecimal](/package/extension5/sspread/properties/typecurrencydecimal)| CRW| ×| UString| ""| Decimal point symbol for currency cell | 
|[TypeCurrencyDecPlaces](/package/extension5/sspread/properties/typecurrencydecplaces)| CRW| ×| integer| 2| Number of digits to display after the decimal point in the currency cell |
|[TypeCurrencyLeadingZero](/package/extension5/sspread/properties/typecurrencyleadingzero)| CRW| ×| integer | $TypeLeadingZeroIntl| Show leading zeros in currency cells |
|[TypeCurrencyMax](/package/extension5/sspread/properties/typecurrencymax)| CRW| ×| Number| 9999999.99| Upper limit that can be entered in currency cell |
|[TypeCurrencyMin](/package/extension5/sspread/properties/typecurrencymin)| CRW| ×| Number | –9999999.99| Lower limit that can be entered in currency cell |
|[TypeCurrencyNegStyle](/package/extension5/sspread/properties/typecurrencynegstyle)| CRW| ×| integer| $TypeCurrencyNegStyleIntl | Negative number format for currency cells |
|[TypeCurrencyPosStyle](/package/extension5/sspread/properties/typecurrencyposstyle)| CRW| ×| integer| $TypeCurrencyPosStyleIntl | Positive format of currency cell |
|[TypeCurrencySeparator](/package/extension5/sspread/properties/typecurrencyseparator)| CRW| ×| UString| ""| Delimiter for every 3 digits of currency cell |
|[TypeCurrencyShowSep](/package/extension5/sspread/properties/typecurrencyshowsep)| CRW| ×| boolean| $FALSE| Display the delimiter for every 3 digits of the currency type cell |
|[TypeCurrencyShowSymbol](/package/extension5/sspread/properties/typecurrencyshowsymbol)| CRW| ×| boolean| $TRUE | Display currency symbol of currency type cell |
|[TypeCurrencySymbol](/package/extension5/sspread/properties/typecurrencysymbol)| CRW| ×| UString | ""| Currency symbol of currency type cell |
|[TypeDateCentury](/package/extension5/sspread/properties/typedatecentury)| CRW| ×| boolean| (OS settings)| 4-digit year display of date cell |
|[TypeDateFormat](/package/extension5/sspread/properties/typedateformat)| CRW| × | integer | (OS settings)|Date cell display format |
|[TypeDateMax](/package/extension5/sspread/properties/typedatemax)| CRW| ×| UString| "20991231"| Upper limit of the date that can be entered in the date cell |
|[TypeDateMin](/package/extension5/sspread/properties/typedatemin)| CRW| ×| UString| "19000101"| Lower limit of the date that can be entered in the date cell |
|[TypeDateSeparator](/package/extension5/sspread/properties/typedateseparator)| CRW| ×| integer |(OS settings) |Date cell date separator |
|[TypeEditCharCase](/package/extension5/sspread/properties/typeeditcharcase) | CRW| ×| integer| $TypeEditCharCaseSetNone| Automatically convert uppercase and lowercase letters in character cells |
|[TypeEditCharSet](/package/extension5/sspread/properties/typeeditcharset)| CRW| ×| integer| $TypeEditCharSetASCII | Character types that can be entered in character cell |
|[TypeEditMultiLine](/package/extension5/sspread/properties/typeeditmultiline)| CRW| ×| boolean| $FALSE| Allow multi-line input for character cells |
|[TypeEditPassword](/package/extension5/sspread/properties/typeeditpassword)| CRW| ×| boolean | $FALSE | Display &#42; instead of the entered character in the character cell |
|[TypeEllipses](/package/extension5/sspread/properties/typeellipses)| CRW| ×| boolean| $FALSE | Display ellipsis in cells that do not fit |
|[TypeHAlign](/package/extension5/sspread/properties/typehalign) | CRW | × | integer |Currency, numbers, percentages, exponential cells<br>$TypeHAlignRight<br>Cell type other than the above<br>$TypeHAlignLeft| Horizontal placement of cells |
|[TypeMaxEditLen](/package/extension5/sspread/properties/typemaxeditlen)| CRW | ×| integer| Character cell<br>32000<br>Combo box type cell<br>150| Maximum number of characters that can be entered in a cell |
|[TypeNegRed](/package/extension5/sspread/properties/typenegred)| CRW| ×| boolean| $FALSE| Negative numbers in cells are displayed in red |
|[TypeNumberDecimal](/package/extension5/sspread/properties/typenumberdecimal)| CRW| ×| UString| ""| Decimal point symbol for numeric cells |
|[TypeNumberDecPlaces](/package/extension5/sspread/properties/typenumberdecplaces)| CRW | ×|integer| 2|  Number of digits to display after the decimal point in a numeric cell |
|[TypeNumberLeadingZero](/package/extension5/sspread/properties/typenumberleadingzero)| CRW| ×| integer| $TypeLeadingZeroIntl| Show leading zeros in numeric cells |
|[TypeNumberMax](/package/extension5/sspread/properties/typenumbermax)| CRW| ×| Number| 9999999.99| Upper limit that can be entered in a numeric cell |
|[TypeNumberMin](/package/extension5/sspread/properties/typenumbermin)| CRW| ×| Number| –9999999.99| Lower limit that can be entered in a numeric cell |
|[TypeNumberNegStyle](/package/extension5/sspread/properties/typenumbernegstyle)| CRW| × | integer | $TypeNumberNegStyleIntl| Negative number format for numeric cells |
|[TypeNumberSeparator](/package/extension5/sspread/properties/typenumberseparator)| CRW| ×| UString | ""| Delimiter for every 3 digits of a numeric cell |
|[TypeNumberShowSep](/package/extension5/sspread/properties/typenumbershowsep)| CRW | × | boolean| $FALSE | Display the delimiter for every 3 digits of the numeric cell |
|[TypePercentDecimal](/package/extension5/sspread/properties/typepercentdecimal)| CRW| ×| UString| ""| Decimal point symbol for percent cell |
|[TypePercentDecPlaces](/package/extension5/sspread/properties/typepercentdecplaces)| CRW| ×| integer| 2|Number of digits to display after the decimal point in the percentage cell  |
|[TypePercentLeadingZero](/package/extension5/sspread/properties/typepercentleadingzero)| CRW| ×| integer| $TypeLeadingZeroIntl | Show leading zeros for percentage cells |
|[TypePercentMax](/package/extension5/sspread/properties/typepercentmax)| CRW| ×| Number| 9999.99| Upper limit that can be entered for percentage cells |
|[TypePercentMin](/package/extension5/sspread/properties/typepercentmin)| CRW| ×| Number| -9999.99| Lower limit that can be entered for percentage cells |
|[TypePercentNegStyle](/package/extension5/sspread/properties/typepercentnegstyle)| CRW| ×| integer| $TypePercentNegStyleIntl| Negative number format for percentage cells |
|[TypePicDefaultText](/package/extension5/sspread/properties/typepicdefaulttext)| CRW| ×| UString| ""| Character string to be displayed instead of the edit definition character of the mask type cell |
|[TypePicMask](/package/extension5/sspread/properties/typepicmask)| CRW| ×| UString| ""|Mask cell format  |
|[TypePictCenter](/package/extension5/sspread/properties/typepictcenter)| CRW| ×| boolean |$FALSE| Center the image of the image type cell |
|[TypePictMaintainScale](/package/extension5/sspread/properties/typepictmaintainscale)| CRW| ×| boolean| $FALSE|  Preserves the aspect ratio of the image in the image type cell |
|[TypePictPicture](/package/extension5/sspread/properties/typepictpicture)| CRW| ×| String<br>Object Reference| - | Image type cell image|
|[TypePictStretch](/package/extension5/sspread/properties/typepictstretch)| CRW| ×| boolean| $FALSE| Enlarging / reducing the image in the image type cell |
|[TypeScientificDecimal](/package/extension5/sspread/properties/typescientificdecimal)| CRW| ×| UString| "" | Decimal point symbol for exponential cells | 
|[TypeScientificDecPlaces](/package/extension5/sspread/properties/typescientificdecplaces)| CRW| ×| integer| 0| Number of digits after the decimal point in the exponential cell |
|[TypeScientificMax](/package/extension5/sspread/properties/typescientificmax)| CRW| ×| Number| 1.7E+308 | Valid maximum value for exponential cells |
|[TypeScientificMin](/package/extension5/sspread/properties/typescientificmin)| CRW| ×| Number | -1.7E+308 | Valid minimum of exponential cells |
|[TypeSpin](/package/extension5/sspread/properties/typespin) | CRW | × | boolean| $FALSE | Show spin button in cell | 
|[TypeSpinInc](/package/extension5/sspread/properties/typespininc) | CRW | × | Number | 1.1 | Amount of change due to one click of the spin button on the cell |
|[TypeSpinWrap](/package/extension5/sspread/properties/typespinwrap) | CRW| × | boolean| $FALSE | Operation at the upper and lower limits of the spin button in the cell |
|[TypeTextOrient](/package/extension5/sspread/properties/typetextorient)| CRW| × | integer| $TypeTextOrientHorizontal | Display direction of cell characters| 
|[TypeTextPrefix](/package/extension5/sspread/properties/typetextprefix) | CRW | × | boolean | $FALSE| Handling of & characters contained in the value of label type cell |
|[TypeTextShadow](/package/extension5/sspread/properties/typetextshadow) | CRW| × | boolean | $FALSE | Convex display of label type cells |
|[TypeTextShadowIn](/package/extension5/sspread/properties/typetextshadowin) | CRW | × | boolean | $FALSE | Concave display of label type cell | 
|[TypeTextWordWrap](/package/extension5/sspread/properties/typetextwordwrap) | CRW | × | boolean | $FALSE | Label type cell word wrap |
|[TypeTime24Hour](/package/extension5/sspread/properties/typetime24hour) |CRW | × | integer| (OS settings) | 12-hour / 24-hour clock cell | 
|[TypeTimeMax](/package/extension5/sspread/properties/typetimemax) | CRW | × | UString | "235959" |Upper limit of time that can be entered in the time cell  |
|[TypeTimeMin](/package/extension5/sspread/properties/typetimemin) | CRW | × | UString | "000000" | Lower limit of time that can be entered in the time cell | 
|[TypeTimeSeconds](/package/extension5/sspread/properties/typetimeseconds) | CRW | × | boolean | $FALSE | Display seconds in time cell |
|[TypeTimeSeparator](/package/extension5/sspread/properties/typetimeseparator) | CRW | × | integer | (OS settings) | Delimiter between hours, minutes, and seconds in a time cell | 
|[TypeVAlign](/package/extension5/sspread/properties/typevalign) | CRW | × | integer | Check box type cell<br>$TypeVAlignCenter<br>Cell type other than the above<br>$TypeVAlignTop |Vertical placement of cells|
|[UseChange](/package/extension5/sspread/properties/usechange) | CRW | | boolean | - | Specifying a value is invalid for this class |
|[UserColAction](/package/extension5/sspread/properties/usercolaction) | CRW | | integer | $UserColActionDefault | The action to take when you click on the column header |
|[UserResize](/package/extension5/sspread/properties/userresize) | CRW | | integer | $UserResizeBoth | Allow mouse to change column width and row height |
|[UserResizeCol](/package/extension5/sspread/properties/userresizecol) |CRW | × | integer | $UserResizeDefault |Allow the mouse to change the width of the column  |
|[UserResizeRow](/package/extension5/sspread/properties/userresizerow) | CRW | × | integer | $UserResizeDefault | Allow mouse to change row height |
|[UseVisualStyles](/package/extension5/sspread/properties/usevisualstyles) | CRW | | integer | $UseVisualStylesInherit | Design of buttons, checkboxes, etc. placed in cells |
| [Value](/package/extension5/sspread/properties/value) |CRW | × | UString | "" | Cell value |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable
