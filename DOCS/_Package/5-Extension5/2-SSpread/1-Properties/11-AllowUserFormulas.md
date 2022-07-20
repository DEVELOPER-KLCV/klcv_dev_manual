---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.AllowUserFormulas Property
nav_order: 11
permalink: /package/extension5/sspread/properties/allowuserformulas
---
# {{ page.title }}

Sets whether users are allowed to enter formulas.

Only cells that have the CellType property set to $CellTypeCurrency (currency type), $CellTypeNumber (numeric type), or $CellTypePercent (percentage type) can be entered formulas.

Specify $TRUE to allow or $FALSE to disallow.

The initial value is $FALSE.

If allowed, the user will be able to set the formula by first entering an equal (=). The formula is displayed in the cell where the formula has already been set and can be edited.

The formula entered can be referenced in the <a href="/package/extension5/sspread/properties/formula">Formula</a> property. (The first equal (=) is not included in the formula)

The <a href="/package/extension5/sspread/events/userformulaentered">UserFormulaEntered</a> event is raised when the user enters the correct formula and the Formula property is updated.

When the formula entered raises a circular reference, it raises the <a href="/package/extension5/sspread/events/circularformula">CircularFormula</a> event.

Set this property to $FALSE to disallow the user to edit the formula.

When this property is set to $ TRUE, the cell has two input modes:

**Formula Input Mode**<br>
The input mode is turned on by first inputting equal (=).

The entered content is retained as a formula, and the result of the formula is displayed on the screen.

**Normal Input Mode**<br>

The input mode is turned on by double-clicking the active cell, pressing the Enter key, or entering characters.

The entered content is retained as cell data and displayed on the screen as it is. The cell data can be referred with the Text property and Value property.

In the normal input mode, the formula can't be set even if equal (=) is entered. The input mode need to be turned off once to enter the formula input mode.

If entered data in the cell where the formula is set in normal input mode, the Formula property does not change, but the screen shows the entered data.

If entered a formula in formula entry mode in a cell with data, the <a href="/package/extension5/sspread/properties/text">Text</a> and <a href="/package/extension5/sspread/properties/value">Value</a> properties are changed to the formula result and the screen displays the formula result.

Related Items<br>
<a href="/package/extension5/sspread/properties/celltype">CellType</a><a href="/package/extension5/sspread/properties/formula">Formula</a>, <a href="/package/extension5/sspread/properties/text">Text</a>, <a href="/package/extension5/sspread/properties/value">Value</a> property <br>
<a href="/package/extension5/sspread/events/circularformula">CircularFormula</a>, <a href="/package/extension5/sspread/events/userformulaentered">UserFormulaEntered</a> event