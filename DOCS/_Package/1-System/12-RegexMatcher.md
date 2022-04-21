---
layout: default

parent: 1. System Package
has_children: true

title: RegexMatcher Class
nav_order: 12
permalink: /package/system/regexmatcher

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

A regular expression engine for interpreting regular expression patterns and performing match operations with input strings.

Objects of RegexMatcher class are created by [Matcher]() method of [RegexPattern]() class. The RegexMatcher class has various methods for match and replace operations.

**<small>[Unicode mode]() can now handle Unicode strings (UString).</small>**

<b>Default properties and ValueType</b>

The default property is [InputString](). The ValueType specification is invalid.

<b>About the reference to the forward reference group of the replace operation method</b>
 
You can refer to the substring of the forward reference group by writing "$n" in the replacement string specified by the [AppendReplacement](), [ReplaceAll](), and [ReplaceFirst]() methods. Describe the group number in n. For example, to refer to group 1, write "$1".

If you want to include "$" as a literal in the replacement string, escape it with "\". When writing in a CRS program, "\" is also an escape character in the CRS program, so it is necessary to overlap two "\" like "\\ $ text".