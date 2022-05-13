---
layout: default
has_children: false

title: Display string and "&" symbol
nav_order: 2
permalink: /base/ampersand
has_toc: false
---

# {{ page.title }}

In the PC version and Mobile version, the "&" symbol may represent an underline in the properties (Title, Value property, etc.) that set the characters displayed on the screen.

If "&" is included in the character string to be set, "&" is not displayed and the next character is underlined.

For example, in the Title property
```
Title = "Print(&P)";
```

Then, the displayed characters are
```
Print(P)
```
An underline is added to P as shown in.

If you want to display the "&" symbol itself, use "&&".
```
Title = "A&&B"; /* Displays A&B */
```

In Windows, pressing the underlined character in combination with the Alt key works like a shortcut function, but in Biz / Browser, this function is not added automatically.

<br>
**<small>The following function is added since Version 5.0.0, Mobile Version 4.5.0</small>*

In a class with the [NoPrefix](/base/base1-28) property defined, you can disable the above behavior and let the "&" sign appear as is.


