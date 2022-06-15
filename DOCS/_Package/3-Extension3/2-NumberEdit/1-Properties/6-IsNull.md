---
layout: default

grand_parent: NumberEdit Class
parent: Properties
has_children: false
title: NumberEdit.IsNull Event
nav_order: 6
permalink: /package/extension3/numberedit/properties/isnull
---
# {{ page.title }}
<br>

When the <a href="/package/extension3/numberedit/properties/format">Format</a> property specifies a format ( N ) that does not display empty data and the Value property is 0 , it is used to determine whether it is 0 entered or cleared with the Delete key.


When you refer to the property, the value is as follows.

| Value  | Description                                 |
|--------|---------------------------------------------|
| $TRUE  | It is in a cleared state by the Delete key  |
| $FALSE | 0 is entered                                |


When a value is set in the property, the behavior is as follows.

| Value  | Description               |
|--------|---------------------------|
| $TRUE  | Hide 0 and leave it blank |
| $FALSE | Display 0                 |

Example
```
NumberEdit num1 {
    Format = "990N";
    Function OnTouch(e) {
        if (Value == 0 && IsNull == $TRUE) {
            MessageBox("何か入力してください");
        }
    }
}
Button btn {
    Title="クリア";
    Function OnTouch(e) {
        ^.num1.IsNull = $TRUE;
    }
}
```


If the Format property does not specify a format (N) that does not display empty data, setting $ TRUE for this property will not result in blanks. Also, when there is a screen operation, it will be $ FALSE.

<br><small><span style="color:red">Added since Ver.4.0.3, Mobile Ver.2.0.0</span></small>