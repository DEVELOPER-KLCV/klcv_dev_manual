---
layout: default

grand_parent: FlexItem Class
parent: Properties
has_children: false
title: FlexItem.TitleFgColor Property
nav_order: 3
permalink: /package/extension4/flexview/flexitem/properties/titlefgcolor
---
# {{ page.title }}

Specifies the text color of the column title.

In addition to the TitleFgColor property, the text color of the title is also affected by the TitleFgColor defined in FlexView. The FlexItem TitleFgColor specification takes precedence, as shown in the following table.

| FlexItem.TitleFgColor | FlexView.TitleFgColor | Display color         |
|-----------------------|-----------------------|-----------------------|
| Unspecified           | Unspecified           | Default color         |
| Unspecified           | Specified             | FlexView.TitleFgColor |
| Specified             | unspecified           | FlexItem.TitleFgColor |
| Specified             | Specified             | FlexItem.TitleFgColor |

TitleFgColor example

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexitemp6.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

```
FlexView FlexView1 {
    :
    TitleFgColor = $3333FF;
    :
    FlexRecord FlexRecord1 {
        :
        FlexColumnSet FlexColumnSet1 {
            :
            Title = "TreeSet";
            TitleFgColor = $FF0000;
            :
            FlexTreeHeader FlexTreeHeader1 {
                Title = "Tree1";
                :
            }
            FlexTreeHeader FlexTreeHeader2 {
                Title = "Tree2";
                :
            }
        }
    }
}
```
<br><small><span style="color:red">Added since Ver.4.1.0</span></small>