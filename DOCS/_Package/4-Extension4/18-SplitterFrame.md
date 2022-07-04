---
layout: default

parent: 4. Extension4 Package
has_children: true

title: SplitterFrame Class
nav_order: 18
permalink: /package/extension4/splitterframe

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-SplitterFrame.PNG" target="_blank">
<img src="/img/Package/Ext4-SplitterFrame.PNG" alt="login image"></a>

A class that displays split frames. A separate form can be placed in each frame and the user can resize it to any size with the touch of a mouse.

The SplitterFrame class works in tandem with the <a href="/package/extension4/splitterform">SplitterForm</a> class.

To set the form to display, you need to place the SplitterForm class or its derived class objects in the structure defined below the SplitterFrame object.

The SplitterFrame class and SplitterForm class are similar in usage and display results to the combination of HTML < FRAMESET > and < FRAME >.

You can create multiple split panes by placing another SplitterFrame object below the SplitterFrame object. 

**Screen Display Example**

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_splitter.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>
 
```

SplitterFrame SplitterFrame1 {
    SplitDirection = $HORIZONTAL;
    SplitterForm SplitterForm1 {
        /* 左 */
    }
    SplitterFrame SplitterFrame2 {
        SplitDirection = $VERTICAL;
        SplitterForm SplitterForm2 {
            /* 右上 */
        }
        SplitterForm SplitterForm3 {
            /* 右下 */
        }
    }
}
```

**Printer output by Doc class**<br>
Not subject to printing.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/splitterframe/properties/value">Value</a>. ValueType can be String, Number, Fixed, Date and UString.<br><small><span style="color:green">Added UString since Ver.4.2.0</span></small>

**Restrictions when visual style is enabled**<br>
Nothing in particular

**Precautions when scaling**<br>
◆ When the SplitterFrame is expanded to eliminate the error of the internal effective area at the time of expansion, it is adjusted to a size slightly smaller than the logically calculated value.

