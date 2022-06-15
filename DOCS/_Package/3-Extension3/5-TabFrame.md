---
layout: default

parent: 3. Extension3 Package
has_children: true

title: TabFrame Class
nav_order: 5
permalink: /package/extension3/tabframe

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext3-TabFrame.PNG" target="_blank">
<img src="/img/Package/Ext3-TabFrame.PNG" alt="login image"></a>


A class that displays tab controls.

The TabFrame class works in tandem with the TabForm class.

To display the tabs, the <a href="/package/extension3/tabform">TabForm</a> class or its derived class objects need to be placed in the structure defined below the TabFrame object.

TabForm objects do not extend beyond the area of the TabFrame object to which they belong and are clipped at the size of the TabFrame object.

**Object Structure**

<a href="/img/Package/Ext3-TabFrame1.PNG" target="_blank">
<img src="/img/Package/Ext3-TabFrame1.PNG" alt="login image"></a>

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext/ext4.files/image002.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

**Printer output by Doc class**<br>
 Not subject to printing. The selected <a href="/package/extension3/tabform">TabForm</a> object will be printed.

**Default properties and ValueType**<br>
 The default property is <a href="/package/extension3/tabframe/properties/value">Value</a>. The value type specification is invalid.
 
**Restrictions when visual style is enabled**<br>
◆ TabPosition can only be used for $STD due to OS restrictions.<br>
◆ BgColor is invalid because it gives priority to the theme display.

 **Precautions when scaling**<br>
◆ Tab scaling only works if the Arrangement property is $STD or $FIXEDWIDTH and TabHeight and TabWidth are non-zero.

<small><span style="color:green">The above restrictions have been removed since Ver.5.0.1.</span></small>