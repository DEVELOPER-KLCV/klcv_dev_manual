---
layout: default

parent: 2. Standard Package
has_children: true

title: TextBox Class
nav_order: 27
permalink: /package/standard/textbox

---
# {{ page.title }}
<br>

<a href="/img/Package/Standard-TextBox.PNG" target="_blank">
<img src="/img/Package/Standard-TextBox.PNG" alt="login image"></a>

A class that displays a text box in which one line of characters can be entered.

The value of the <a href="/package/standard/textbox/properties/value">Value</a> property is formatted and displayed in the text box according to the specification of the <a href="/base/format">Format</a> property.

When inputting, the specification of the Format property becomes invalid and the format corresponding to the value data type is input.

<br><small><span style="color:green">It is possible to switch between insert mode and overwrite mode using the Insert key since Ver.5.0.0</span></small>

**Screen Display Example**


{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std3.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Input Format according to Data Type**<br>
The TextBox class supports input according to ValueType, so when it receives keyboard focus, it invalidates the specification of the Format property and prompts for input in a format corresponding to the data type.

<a href="/img/Package/Standard-TextBox1.PNG" target="_blank">
<img src="/img/Package/Standard-TextBox1.PNG" alt="login image"></a>

The input formats for each Value Type are shown below.

<ol>

<li>String</li>

The value of the Value property is displayed as is and you can enter it.

<li>Date</li>

The input format varies depending on what the value of the Value property is at the start of input. <br>

   	(1) If the hour, minute, and second of the value of the Value property are all 00, the format is "YYYY / MM / DD".<br>
    
    (2) If the value of the Value property has a second of 00, it will be in the "YYYY / MM / DD HH24: MI" format.<br>
    
    (3) In cases other than the above, it will be in "YYYY / MM / DD HH24: Mi: SS" format.<br>


<li> Number</li>

Enter the value of the Value property, which is displayed in all digits including the digits after the decimal point.

 
<li> UString <small><span style="color:red">Added since Ver.4.2.0</span></small> </li> <br>

The value of the Value property is displayed and entered as is. The character code of the value of the Value property is Unicode.

In Windows98 and ME, since the Unicode input function at the OS level is not supported, it is not possible to input or display Unicode-specific characters, and it cannot be specified together with the <a href="/package/standard/editbox/properties/maxlength">MaxLength</a> property. 
</ol> 
 
**Printer Output by Doc class**<br>
Enclose the characters in a square and display them.

Even if the UString type is specified, all characters are converted to multibyte when printing, so Unicode-specific characters are printed as "?".

**Default properties and ValueType**<br>

The default property is <a href="/package/standard/textbox/properties/value">Value</a> . ValueType can be String, Number, Fixed, Date and UString.<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small><br><br>

**Restrictions when visual style is enabled** <br>
Nothing in particular.<br><br>

**Precautions when scaling** <br>
Nothing in particular.