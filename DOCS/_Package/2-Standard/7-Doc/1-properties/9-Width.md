---
layout: default

grand_parent: Doc Class
parent: Properties
has_children: false
title: Doc.Width property
nav_order: 9
permalink: /package/standard/doc/properties/width
---
# {{ page.title }}


The width of the paper. The initial value is automatically determined by the Format property.


| Format  Property | Width x Height (Dot unit) | Paper size mm (Horizontal x Vertical) |
|------------------|---------------------------|---------------------------------------|
| A4V              | 793 x 1122                | 2100 x 2970                           |
| A4H              | 1122 x 793                | 2970 x 2100                           |
| A5V              | 599 x 793                 | 1480 x 2100                           |
| A5H              | 793 x 599                 | 2100 x 1480                           |
| A3V              | 1122 x 1587               | 2970 x 4200                           |
| A3H              | 1587 x 1122               | 4200 x 2970                           |
| B5V              | 687 x 971                 | 1820 x 2570                           |
| B5H              | 971 x 687                 | 2570 x 1820                           |
| B4V              | 971 x 1375                | 2570 x 3640                           |
| B4H              | 1375 x 971                | 3640 x 2570                           |

If you set values for the Width and Height properties, the values will be scaled to fit the paper size.

```
Doc Doc1 {
    Format = "A4H";
    Form Form1 {
        Width = 400;
        Height = 400;
        Label Label1 {
            Width = 80;
            Height = 30;
            Border = $ TRUE;
        }
    }
}
```

Doc 1 preview

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21p2.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>


```
Doc Doc2 {
    Format = "A4H";
    Form Form1 {
        Width = 400;
        Height = 400;
        Label Label1 {
            Width = 80;
            Height = 30;
            Border = $TRUE;
        }
    }
    if (!$DESIGNTIME) {
        Width = Form1.Width;
        Height = Form1.Height;
    }
}
```

Doc 2 preview

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21p2.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

