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

### Get sort status

The sort state of a column can be obtained when sorting is allowed in the UserColAction property.
```
if (ColUserSortIndicator (2) == $ ColUserSortIndicatorAscending) {
    MessageBox (" Sort in ascending order in the second column ");
} else if (ColUserSortIndicator (2) == $ ColUserSortIndicatorDescending) {
    MessageBox (" Sort in descending order in the second column ");
} else if (ColUserSortIndicator (2) == $ ColUserSortIndicatorNone) {
    MessageBox (" Not sorted in second column ");
}
```

If $UserColActionSortNoIndicator is set in the UserColAction property, the sort indicator (△ ▽ mark in the column header) will not be displayed, but the sort status can be obtained with the ColUserSortIndicator property.

### Prohibit sorting certain columns

Certain columns can be prevented from sorting by specifying $ ColUserSortIndicatorDisabled for the ColUserSortIndicator property when sorting is allowed in the UserColAction property.

```
UserColAction = $ UserColActionSort;
/ * Do not sort the 2nd and 3rd columns * /
ColUserSortIndicator (2) = $ ColUserSortIndicatorDisabled;
ColUserSortIndicator (3) = $ ColUserSortIndicatorDisabled;
```

### Sort by program

If you want to sort from the CRS program instead of user operation, set the UserColAction property after setting the ColUserSortIndicator property.

```
/ * Sort in ascending order in the second column * /
ColUserSortIndicator (2) = $ ColUserSortIndicatorAscending;
UserColAction = $ UserColActionSort;
```
Do not set the ColUserSortIndicator property for multiple columns, as sorting is done with a specific column as the key.

### Switch the sort indicator display

When $UserColActionSort is specified in the UserColAction property, the sort indicator (△ ▽ mark in the column header) displayed in the column header in the ColUserSortIndicator property can be changed. There is no sorting.

```
UserColAction = $ UserColActionSort;
ColUserSortIndicator (2) = $ ColUserSortIndicatorAscending;
ColUserSortIndicator (3) = $ ColUserSortIndicatorDescending;
```

Related Item<br>
<a href="/package/extension5/sspread/properties/usercolaction">UserColAction</a> property
