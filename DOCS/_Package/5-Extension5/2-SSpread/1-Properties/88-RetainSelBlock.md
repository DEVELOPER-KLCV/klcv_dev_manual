---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.RetainSelBlock Property
nav_order: 88
permalink: /package/extension5/sspread/properties/retainselblock
---
# {{ page.title }}

Sets whether to keep the selection and highlighting of active cells when the spreadsheet loses focus.

Specify the following values. The initial value is $FALSE.

| Constant | Description                            |
|----------|----------------------------------------|
| $TRUE    | Keep highlighting even when lose focus |
| $FALSE   | Remove highlight when out of focus     |

If $FALSE is specified, the highlighting will be temporarily canceled when the focus is lost, but it will be restored when the focus is regained. (The selected state is not canceled)