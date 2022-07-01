---
layout: default

grand_parent: ListViewSubItem Class
parent: Properties
has_children: false
title: Format Property
nav_order: 3
permalink: /package/extension4/listviewsubitem/properties/format
---
# {{ page.title }}
<br>

Specify the format of the edit string for each data type.

***Specified characters that can be used in common in all formats***

| Specified Character | Example             | Description                                                                                                                                                                                                           |
|:-------------------:|---------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|          @          | "￥"Maximum￥"@"   | Display in the specified position in the default format. If the data type is Date, @d displays the date only, @t displays the time without the date and seconds, and @s displays the time with the date and seconds. |
|        "TEXT"       | "9990￥" 円￥ ""   | The characters enclosed in "" are displayed at the specified position. When specified for Number type or Fixed type data, it cannot be specified at the position that separates the sequence of numbers.              |

<br>

***If the data type is String, UString***

| Specified Character | Example | Description                                                                                                                                                                                                     |
|:-------------------:|:-------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|         Sn.m        |  "S2.3" | The left end of the character string is counted as 0, and the characters from the n<sup>th</sup> byte to the m<sup>th</sup> byte are displayed. For UString, the n<sup>th</sup> to m characters are displayed. |

<br>

***If the data type is Number, Fixed***

| Specified Character |     Example     | Description                                                                                                                                                                                                     |
|:-------------------:|:---------------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|          9          |     "999"       | The number that describes 9 indicates the number of digits, and the leading 0 is deleted. If specified after the decimal point, it means only the number of digits and zero suppression is not performed.       |
|          0          |  "0999" "9990"  | Leading 0 is 0.                                                                                                                                                                                                 |
|          $          |    "$ 9990"     | Add a $ mark at the beginning.                                                                                                                                                                                  |
|          MI         | "999MI" "MI999" | For negative numbers, a minus sign ( - ) is displayed at the specified position (right or left).                                                                                                                |
|          S          | "S9990" "9990S" | The sign is displayed at the specified position (right or left).                                                                                                                                                |
|   D or . (Period)   | "99D99" "99.99" | Displays the decimal point at the specified position. If you do not specify the number of digits after the decimal point, the last digit within the valid accuracy range is displayed.                          |
|          L          | "L9990" "9990L" | Displays the local currency symbol at the specified position (right or left).                                                                                                                                   |
|      , (Comma)      |   "999,990"     | Displays a comma every 3 digits.                                                                                                                                                                                |
|     "" ( Space )    |    "    99"     | The number that describes the space indicates the number of digits, and the leading 0 is replaced with a blank character (space). If it is specified after the decimal point, it is invalid and has no meaning. |
|          !!         |     "999!"      | If an overflow occurs within the specified number of digits, the formatted result will be displayed with a !, But if you specify!, The display of! Will be suppressed even if the overflow occurs .             |

<br>

***If the data type is Date***

| Specified Character |                      Example                      | Description                                                                                                                               |
|:-------------------:|:-------------------------------------------------:|-------------------------------------------------------------------------------------------------------------------------------------------|
|          Y          | "YYYY, MM, DD"                                    | Displays the year of the Christian era. The number in which Y is described indicates the number of digits displayed in the Christian era. |
|          WS         | "WSWYY.MM.DD"                                     | Displays the Japanese era in abbreviations ( M, T, S, H ... ).                                                                            |
|          WR         | "WRWYY \" year \ "MM \" month \ "DD \" day \ ""   | The year of the Japanese calendar is displayed (Meiji, Taisho, Showa, Heisei, Reiwa .. ). <br><small><span style="color:green">Added "Reiwa" since Ver.5.1.1</span></small>
|         WYY         | "WRWYY \" year \ "MM \" month \ "DD \" day \ ""   | Displays the year of the Japanese calendar.                                                                                               |
|          MM         | "YYYY / MM"                                       | Displays the month ( 1 to 12 ).                                                                                                           |
|        MONTH        | "MONTH DD YYYY"                                   | Displays the name of the month ( JANUARY ... ). It is displayed in 9 digits.                                                              |
|        month        | "month DD YYYY"                                   | Displays the name of the capitalized month ( January ... ). It is displayed in 9 digits. <br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>                                     |
|         MON         | "dy, DD MON YYYY"                                 | Displays the abbreviation ( JAN ... ) for the name of the month.                                                                          |
|         mon         | "dy, DD mon YYYY"                                 | Displays the abbreviation ( Jan ... ) for the name of the capitalized month. <br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>              |
|          DD         | "YY / MM / DD"                                    | Displays the day ( 1 to 31 ).                                                                                                             |
|         DAY         | "YY / MM / DD DAY"                                | Displays the day of the week ( SUNDAY ... ).                                                                                              |
|         day         | "YY / MM / DD day"                                | Displays the capitalized day of the week ( Sunday ... ). <br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>                                                |
|          DY         | "YY / MM / DD DY"                                 | Displays the abbreviation for the day of the week ( SUN ... ).                                                                            |
|          dy         | "dy, DD mon YYYY"                                 | Displays the capitalized day of the week abbreviation ( Sun ... ). <br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>                            |
|          DJ         | "YY / MM / DD DJ"                                 | Displays the local form of the day of the week (Monday, Tuesday ... ).                                                                    |
|          HH         | "HH: MI: SS"                                      | Displays the time of the 12 -hour system ( 0 to 11 ).                                                                                     |
|         HH24        | "HH24: MI: SS"                                    | 24. Displays the time system ( 0 to 23 ).                                                                                                 |
|          MI         | "HH: MI: SS"                                      | Displays the minute ( 0 to 59 ).                                                                                                          |
|          SS         | "HH: MI: SS"                                      | Displays seconds ( 0 to 59 ).                                                                                                             |
|          TZ         | "HH24: MI: SS TZ"                                 | Displays the time zone in the format +0900 . <br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>                                                                   |
|         u u         | "YY / MM / DD uHH24: MI: SS"                      | Displays the values after the specified location in UTC format. <br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>                                   |
|        -/,.;:       | "HH: MI: SS"                                      | Displays the specified character at the specified position.                                                                               |

※ WS, WR, WYY can be used only in areas where the Japanese calendar is valid.

※ When using the year of the Japanese calendar with WS, WR, and WYY, it is necessary to set the year information in advance with the <a href="/package/standard/root/methods/setwareki">Root.SetWareki</a> method. It is set automatically from Meiji to Reiwa.

※ It is not possible to specify a day such as DAY or-/,.;: alone. Be sure to use these in combination with the formats that you can enter.
