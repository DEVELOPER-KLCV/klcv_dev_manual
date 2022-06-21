---
layout: default

grand_parent: FlexItem Class
parent: Properties
has_children: false
title: FlexItem.TitleBgColor Property
nav_order: 2
permalink: /package/extension4/flexview/flexitem/properties/titlebgcolor
---
# {{ page.title }}

Specifies the background color for the column title.

The background color of the title is influenced by the TitleBgColor property as well as the TitleBgColor defined in FlexView. The FlexItem TitleBgColor specification takes precedence, as shown in the following table.

| FlexItem.TitleBgColor | FlexView.TitleBgColor | Display color         |
|-----------------------|-----------------------|-----------------------|
| Unspecified           | Unspecified           | Default color         |
| Unspecified           | Specified             | FlexView.TitleBgColor |
| Specified             | unspecified           | FlexItem.TitleBgColor |
| Specified             | Specified             | FlexItem.TitleBgColor |


TitleBgColor example

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/ext4/ext_flexitemp5.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

```
FlexView FlexView1 {
    :
    TitleBgColor = $6666FF;
    :
    FlexRecord FlexRecord1 {
        :
        FlexColumnSet FlexColumnSet1 {
            :
            Title = "TreeSet";
            TitleBgColor = $33FF33;
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