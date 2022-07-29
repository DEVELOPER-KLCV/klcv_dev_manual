---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ScrollBarTrack Property
nav_order: 104
permalink: /package/extension5/sspread/properties/scrollbartrack
---
# {{ page.title }}

Sets whether to scroll the contents of the spreadsheet while manipulating the scroll box on the scroll bar.

Specify the following values. The initial value is $ScrollBarTrackOff.

| Constant                  | Value | Description              |
|---------------------------|:-----:|--------------------------|
| $ScrollBarTrackOff        |   0   | Do not scroll            |
| $ScrollBarTrackVertical   |   1   | Scroll only vertically   |
| $ScrollBarTrackHorizontal |   2   | Scroll only horizontally |
| $ScrollBarTrackBoth       |   3   | Scroll all               |

With the $ ScrollBarTrackOff setting, the spreadsheet display does not change while scrolling by dragging the scroll box. The display will be updated when the drag is finished.

Specify something other than $ScrollBarTrackOff, in order the spreadsheet contents to be displayed while scrolling.

Related Item<br>
<a href="/package/extension5/sspread/properties/scrollbars">ScrollBars</a> property

