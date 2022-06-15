---
layout: default

parent: 3. Extension3 Package
has_children: true

title: NumberEdit Class
nav_order: 2
permalink: /package/extension3/numberedit

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext3-NumberEdit.PNG" target="_blank">
<img src="/img/Package/Ext3-NumberEdit.PNG" alt="login image"></a>

A class that displays a text box dedicated to numerical input. There is a simple calculator function that supports the input of numerical values.

<br><small><span style="color:red">Simple calculator is now available since Mobile Ver.3.0.0</span></small>
<br><small><span style="color:blue">Simple calculator cannot be used with AI</span></small>

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext2.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


**Simple Calculator**<br>
Press the space key to activate the calculator. Press Shift + Space to start the calculator with the current value as the initial value.

(In the Mobile version, it is displayed when the a href="/package/extension3/DateEdit/methods/showhelper">ShowHelper</a> method is executed.)

You can enter up to 15 digits excluding the sign and decimal point.

The [CE / C] button clears the previous operation if it is in the middle of calculation, and zeros if the calculation is confirmed.

The [=] button confirms the calculation if it is in the middle of calculation, transfers the result to the NumberEdit object if the calculation is confirmed, and closes the calculator.


**Precautions when using a simple calculator**<br>
Even if the format of the edit character string is specified in the Format property, the contents of the Format property will not be reflected in the simple calculator.

Therefore, it is possible to input in a format that does not conform to the set format on the simple calculator, but the value on the simple calculator is changed to the format set when it is reflected in NumberEdit, so the value different from the input value on the calculator may be displayed.

Example<br>

Format = "999,990"; ※ Cannot be entered after the decimal point
Input on a simple calculator: 1.05
Display when reflected in NumberEdit: 105

**Simple Calculator Keyboard Operation**<br>
In addition to operating buttons with the mouse on the calculator, you can also input from the keyboard.

| Numeric key<br>Numeric keypad<br>Four arithmetic operations symbols | Entering and calculating values                  |
|---------------------------------------------------------------------|--------------------------------------------------|
| BackSpace                                                           | Delete one character                             |
| Delete                                                              | [CE / C] button                                  |
| Esc                                                                 | Cancel the value and close the calculator window |
| Enter                                                               | [=] button                                       |
| R                                                                   | [1 / X] button                                   |
| @                                                                   | [SQR] button                                     |
| F9                                                                  | [+/-] button                                     |
| %%                                                                  | [%] Button                                       |
| Ctrl + P                                                            | [M +] button                                     |
| Ctrl + N                                                            | [M-] button                                      |
| Ctrl + R                                                            | [RM] button                                      |
| Ctrl + L                                                            | [CM] button                                      |

<br><small><span style="color:green">The shape of the calculator has changed from Ver.4.1.0. As a result, the operability has also changed.</span></small>

**Input Digit Limit**<br>
Limiting the number of input digits includes specifying the <a href="/package/extension3/numberedit/properties/format">Format</a> property and <a href="/package/extension3/numberedit/properties/maxlength">MaxLength</a> property.

If the number of digits of the decimal point or integer such as "999." or ".00" is not set in the Format property, the input limit will be applied based on the MaxLength property. For example, when the MaxLength property is the initial value (15), if it is "999.", the digit after the decimal point is 12 digits (15-3), and if it is ".00", the digit of the integer is 13 digits (15-2). ).

If a value less than or equal to the number of digits in the Format property is set in the MaxLength property, the number of digits in the Format property takes precedence.

If neither digit is specified in the Format property, the total length is limited to not exceed the MaxLength property.

The <a href="/package/extension3/numberedit/properties/autotab">AutoTab</a> property works with this input digit limit.

**Printer output by Doc class**<br>
 It will be printed in the same way as the screen.


**Default properties and ValueType**<br>
 The default property is <a href="/package/extension3/numberedit/properties/value">Value</a>. The value type specification is invalid.

 
**Restrictions when visual style is enabled**<br>
 Nothing in particular


 **Precautions when scaling**<br>
◆ Calculator window is not subject to scaling