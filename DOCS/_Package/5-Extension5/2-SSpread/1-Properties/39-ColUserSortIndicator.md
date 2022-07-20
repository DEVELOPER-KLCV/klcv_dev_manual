---
layout: default

grand_parent: SSpread Class
parent: Properties
has_children: false
title: SSpread.ColUserSortIndicator Property
nav_order: 39
permalink: /package/extension5/sspread/properties/colusersortindicator
---
# {{ page.title }}

Set each column for sorting by column header.

This property is an <a href="package/extension5/sspread/#index-property-">Index Property</a>. Specify the column number for the index.

Specify the following values. The initial value is $ColUserSortIndicatorNone.

| Constant                        | Value | Description               |
|---------------------------------|:-----:|---------------------------|
| $ColUserSortIndicatorNone       |   0   | None                      |
| $ColUserSortIndicatorAscending  |   1   | Sort △ (ascending order)  |
| $ColUserSortIndicatorDescending |   2   | Sort ▽ (descending order) |
| $ColUserSortIndicatorDisabled   |   3   | Sorting disabled          |

Use this property in conjunction with the <a href="/package/extension5/sspread/properties/usercolaction">UserColAction</a> property. If the UserColAction property is set to $UserColActionSort, $UserColActionSortNoIndicator, the user can sort by clicking on the column header. Sorting is done for the entire spreadsheet, keyed by one particular column.