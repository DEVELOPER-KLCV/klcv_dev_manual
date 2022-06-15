---
layout: default

grand_parent: NumberEdit Class
parent: Properties
has_children: false
title: NumberEdit.Format Event
nav_order: 4
permalink: /package/extension3/numberedit/properties/format
---
# {{ page.title }}
<br>

Specifies the format of the edit string.

| Specified Character | Example            | Description                                                                                                                                                                                                     |
|---------------------|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| @                   | "\" Max \"@"<br>   | Display in the specified position in the default format.                                                                                                                                                        |
| "TEXT"              | "9990\"円\""<br>   | The characters enclosed in "" are displayed at the specified position. It cannot be specified at the position that separates the sequence of numbers.                                                           |
| 9                   | "999"<br>          | The number that describes 9 indicates the number of digits, and the leading 0 is deleted. If specified after the decimal point, it means only the number of digits and zero suppression is not performed.       |
| 0                   | "0999"<br>"9990"   | Leading 0 is 0 .                                                                                                                                                                                                |
| $                   | "$9990"<br>        | Add a $ mark at the beginning .                                                                                                                                                                                 |
| MI                  | "999MI"<br>"MI999" | For negative numbers, a minus sign ( - ) is displayed at the specified position (right or left).                                                                                                                |
| S                   | "S9990"<br>"9990S" | The sign is displayed at the specified position (right or left).                                                                                                                                                |
| D or<br>. (Period)  | "99D99"<br>"99.99" | Displays the decimal point at the specified position. If you do not specify the number of digits after the decimal point, the last digit within the valid accuracy range is displayed.                          |
| L                   | "L9990"<br>"9990L" | Displays the local currency symbol at the specified position (right or left).                                                                                                                                   |
| , (Comma)           | "999,990"<br>      | Displays a comma every 3 digits.                                                                                                                                                                                |
| "" ( Space )        | "   99"<br>        | The number that describes the space indicates the number of digits, and the leading 0 is replaced with a blank character (space). If it is specified after the decimal point, it is invalid and has no meaning. |
| N                   | "990N"<br>         | Does not display empty data.<br>Added since <img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/ver-add403.gif" alt="Image" width="50" height="12"><img src="https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/ver_images/mver-add200.gif" alt="Image" width="86" height="12">                                                                                                                                                                   |

