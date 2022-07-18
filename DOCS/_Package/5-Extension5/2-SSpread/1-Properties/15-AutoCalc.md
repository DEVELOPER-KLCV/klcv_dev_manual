---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ArrowAutoCalcsExitEditMode Property
nav_order: 15
permalink: /package/extension5/sspread/properties/autocalc
---
# {{ page.title }}

Sets whether to automatically recalculate each formula in the related cell each time a value in the cell's been entered or changed.

Specify $TRUE for recalculation, $FALSE otherwise. The initial value is $TRUE.

The formula in the cell is set in the <a href="/package/extension5/sspread/properties/formula">Formula</a> property.

If $FALSE is set, the formula will not be recalculated automatically and will be recalculated by the <a href="/package/extension5/sspread/methods/recalc">ReCalc</a> method. Use the <a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a> method to recalculate the formula for a particular cell.

Automatically update cell references (such as A1) in formulas by adding or removing columns or rows is set in the  <a href="/package/extension5/sspread/properties/formulasync">FormulaSync</a> property.

Related Items<br>
<a href="/package/extension5/sspread/properties/formula">Formula</a>, <a href="/package/extension5/sspread/properties/formulasync">FormulaSync</a> property<br>
<a href="/package/extension5/sspread/methods/recalc">ReCalc</a>, <a href="/package/extension5/sspread/methods/recalccell">ReCalcCell</a> method