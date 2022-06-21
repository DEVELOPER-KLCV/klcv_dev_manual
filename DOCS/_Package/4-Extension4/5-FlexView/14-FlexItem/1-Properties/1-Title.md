---
layout: default

grand_parent: FlexItem Class
parent: Properties
has_children: false
title: FlexItem.Title Property
nav_order: 1
permalink: /package/extension4/flexview/flexitem/properties/title
---
# {{ page.title }}

Specifies the column title.

If you specify UString for ValueType, this property behaves as a UString type. <br><small><span style="color:red">Added since Ver.5.0.3</span></small>

FlexColumnSet and FlexRowSet titles are displayed separately from the underlying FlexItem.

If you do not want to display the title, set the string "null". Even if null is set, it becomes "null" due to character string conversion, so it is synonymous.

If "null" is set, it will be hidden including the title frame, and if possible, the display area will not be allocated.

Display example when Title = null is not specified<br>
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexitemp2.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

Display example when Title = null is specified<br>
{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexitemp2.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

Script example

```
FlexRecord FlexRecord1 {
    FlexHeader header {
        Numbered = $TRUE;
    }
    FlexLabel FlexLabel4 {
        Title = "Label4";
    }
    FlexRowSet RowSet1 {
        Title = null;
        FlexColumnSet ColSet1 {
            Title = null;
            FlexLabel FlexLabel2 {
                Title = "Label2";
            }
            FlexLabel FlexLabel3 {
                Title = "Label3";
            }
        }
        FlexLabel FlexLabel4 {
            Title = "Label4";
        }
    }
}
```