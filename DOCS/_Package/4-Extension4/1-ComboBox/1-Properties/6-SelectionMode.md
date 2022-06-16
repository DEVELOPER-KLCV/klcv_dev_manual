---
layout: default

grand_parent: ComboBox Class
parent: Properties
has_children: false
title: ComboBox.SelectionMode Property
nav_order: 6
permalink: /package/extension4/combobox/properties/selectionmode
---
# {{ page.title }}
<br>

Specify how to select from the options.

Specify with a combination of the following values.

| Constant   | Value | Description                                                                                        |
|------------|:-----:|----------------------------------------------------------------------------------------------------|
| $NOCASE    |   1   | Do not distinguish between uppercase and lowercase letters when searching for options by keystroke |
| $CLEARABLE |   2   | Allow a state where nothing is selected                                                            |

Specifying $CLEARABLE allows unselected even if the Editable property is $FALSE.