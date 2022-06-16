---
layout: default

grand_parent: ComboBox Class
parent: Properties
has_children: false
title: ComboBox.Value Property
nav_order: 7
permalink: /package/extension4/combobox/properties/value
---
# {{ page.title }}
<br>

The value to be displayed in the text box part of the combo box.

If the <a href="/package/extension4/combobox/properties/editable">Editable</a> property is $FALSE, you can only enter values defined in the <a href="/package/extension4/comboitem">ComboItem</a> object of choice from the screen. If the input confirmation operation is performed while a value other than the options is being input, the input is canceled and the previous state is restored.

Scripted value settings are not affected by the <a href="/package/extension4/combobox/properties/inputmode">InputMode</a> property.

The input value on the screen is not reflected immediately. Refer to the <a href="/package/standard/editobject/#timing-the-value-property-updated">Timing the Value Property Updated</a> for more information.