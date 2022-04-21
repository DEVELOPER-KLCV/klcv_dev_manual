---
layout: default

parent: 1. System Package
has_children: true

title: Record Class
nav_order: 11
permalink: /package/system/record

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

A class for grouping multiple objects. 

The Record class itself has no functionality and is used to place and organize other objects underneath the Record object.

For example, you can use the Record class to return structured data in the return value of a Function.

``` 
Function sample () {
    var ret = new Record {
        Number code;
        String text;
    }
    ret.code = 100;
    ret.text = "abcdefg";
    return ret;
}
``` 

It can also be used when you want to create a simple data structure with a CRS program.

 
```
Record custDB [] {
    Number cust Code;
    String custName;
    String custAddr;
}
custDB << CSV {
    1001, "Tokyo Taro", "Tokyo"
    1002, "Osaka Hanako", "Osaka Prefecture"
    :
};
```

<b>Default properties and ValueType</b>
 
The default property is [Value](). The ValueType specification is invalid.