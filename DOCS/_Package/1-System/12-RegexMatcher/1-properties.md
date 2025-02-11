---
layout: default

grand_parent: 1. System Package
parent: RegexMatcher Class

title: Properties
nav_order: 1
permalink: /package/system/regexmatcher/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the RegexMatcher class.

|Name       | Access | Type   | Description |
|----------	|:--------:|--------|-------------|
|[GroupCount](/package/system/regexmatcher/properties/groupcount) | R | integer |Number of forward reference groups specified in the regular expression pattern |
|[InputString](/package/system/regexmatcher/properties/inputstring)* | R|String |Input string set in the regular expression engine |
|[Pattern](/package/system/regexmatcher/properties/pattern) | R | RegexPattern |RegexPattern object from which the RegexMatcher object was created |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property