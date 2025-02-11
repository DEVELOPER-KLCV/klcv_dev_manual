---
layout: default

grand_parent: FlexCheckButton Class
parent: Properties
has_children: false
title: FlexCheckButton.Active Property
nav_order: 1
permalink: /package/extension4/flexview/flexcheckbutton/properties/active
---
# {{ page.title }}

Specifies the initial value of the activity of the check button on the cell.

The value of the Active property is used as the initial value of the activity to display in the cells of each row generated by the FlexView.InsertRow method. You can also change the activity of all existing rows at once by updating the Active property.

To change the activity of a particular cell, get the FlexRow object in the row you want to change and set the Active property of the FlexCheckButtonCell object that will be placed as a child object of FlexRow with the same name as the corresponding FlexCheckButton object.

If set to true, the button can be operated.
If false is specified, button operations are prohibited.