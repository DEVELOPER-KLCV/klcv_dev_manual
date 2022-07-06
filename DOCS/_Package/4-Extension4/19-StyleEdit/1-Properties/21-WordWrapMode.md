---
layout: default

grand_parent: StyleEdit Class
parent: Properties
has_children: false
title: StyleEdit.WordWrapMode Property
nav_order: 21
permalink: /package/extension4/styleedit/properties/wordwrapmode
---
# {{ page.title }}

This property is meaningful only when the WordWrap property is set to true, and specifies the rule for determining the automatic line feed position.

Specify this property in any combination of the following values:

| Constant | Description                                                                                                                                                                          |
|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| $CHAR    | The line feed position is in character units.                                                                                                                                        |
| $WORD    | The line feed position is in word units. Double-byte characters such as whitespace, tab characters, character decoration boundaries, and Japanese are identified as word boundaries. |
| $KINSOKU | Enables line-breaking and line-end kinsoku processing.                                                                                                                               |

The above values can be specified in combination, and a line break will occur at a position that meets all the specified conditions. For example, if $ WORD + $ KINSOKU is specified, a line break will occur at the position where the prohibition processing is performed at the word boundary.

The prohibited characters considered by $ KINSOKU are the characters listed in the head_kinsoku element and tail_kinsoku element described in the system.xml file under the Biz / Browser installation folder. By default, the following characters are targeted.

Forbidden characters at the beginning of a line<br>
```
!%),.:;?]}?°’”‰′″℃、。々〉》」』】〕ぁぃぅぇぉっゃゅょゎ゛゜ゝゞ
ァィゥェォッャュョヮヵヶ・ーヽヾ！％），．：；？］｝｡｣､･ｧｨｩｪｫｬｭｮｯｰﾞﾟ￠
```

End-of-line forbidden characters<br> 
```
$([\\{??‘“〈《「『【〔＄（［｛｢￡￥
```

In addition, these prohibited characters have different character sets depending on the language of the OS in which they are executed.

<small><span style="color:red">Added since Ver.4.2.0</span></small>
