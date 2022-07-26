---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.FormulaSync Property
nav_order: 61
permalink: /package/extension5/sspread/properties/formulasync
---
# {{ page.title }}

Sets whether cell references (such as A1) in formulas are automatically updated when rows or columns are added, deleted, or moved.

Specify $TRUE to automatically update cell references in formulas, otherwise $FALSE. The initial value is $TRUE.

Set $TRUE to automatically update cell references in formulas when cell positions change due to additions, deletions, cell block movements, etc. of rows and columns.

Set $FALSE, the formula will not be updated when the cell position changes.

The cell formula is set with the <a href="/package/extension5/sspread/properties/formula">Formula</a> property.

The automatic recalculation of formulas is set in the <a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a> property.

Related Items<br>
<a href="/package/extension5/sspread/properties/autocalc">AutoCalc</a>, <a href="/package/extension5/sspread/properties/formula">Formula</a> property