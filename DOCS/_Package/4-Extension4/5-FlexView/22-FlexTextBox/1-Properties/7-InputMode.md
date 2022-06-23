---
layout: default

grand_parent: FlexTextBox Class
parent: Properties
has_children: false
title: InputMode Property
nav_order: 7
permalink: /package/extension4/flexview/flextextbox/properties/inputmode
---
# {{ page.title }}

Specify the character types that can be entered.

|Constant | Value  | Description         | Character code in UString |
|---------|--------|---------------------|---------------------------|
|$STD     | 0      | All character types | ‐                         |
|$NUMERIC | 1      |Half-width numbers, half-width spaces<br>0～9 | U+0030～U+0039 |
| $ALPHA  | 2      | Half-width alphabet, half-width space<br>a～z、A～Z | U+0041～U+005A、U+0061～U+007A|
| $SYMBOL | 4      | Half-width symbols (half-width numbers, half-width characters other than half-width alphabets), half-width spaces<br>!"#$%&'()=~&#124;\^-@[]:;,./\_?><+*{}` | U+0021～U+002F、U+003A～U+0040、<br>U+005B～U+0060、U+007B～U+00FE、<br>U+F8F0、U+FF61～U+FF65 |
| $KANA   | 8       | Half-width katakana, half-width space<br>ｱ～ﾝ | U+FF66～U+FF9F |
| $DNUMERIC | 16 | Full-width numbers, full-width / half-width spaces<br>０～９ | U+FF10～U+FF19 |
| $DALPHA  | 32   | Full-width alphabetic characters, full-width / half-width spaces<br>ａ～ｚ、Ａ～Ｚ | U+FF21～U+FF3A、U+FF41～U+FF5A |
| $DSYMBOL | 64 | Full-width symbols (full-width katakana, full-width hiragana, full-width Chinese characters, full-width numbers, full-width characters other than full-width alphabetic characters), full-width / half-width spaces<br>！“＃＄％＆‘（）＝～ &#124;｀｛｝&#42;＋＜＞？＿￥・。、「」：；＠ | Not applicable to others |
| $DKANA | 128 | Full-width katakana, full-width / half-width space | U+30A1～U+30FA、U+30FC～U+30FF、<br>U+31F0～U+31FF |
| $DHIRA | 256 |Full-width hiragana, full-width and half-width spaces | U+3041～U+3096、U+3099～U+309F |
| $DKANJI | 512 |Full-width Chinese characters, full-width / half-width spaces | U+4E00～U+ABFF、U+F900～U+FAFF |
| $HANKAKU | 15 | Half size | Applicable to $NUMERIC、$ALPHA、$SYMBOL、$KANA |
|$ZENKAKU | 1008 | Full-width, full-width / half-width space |  Applicable to  $DNUMERIC、$DALPHA、$DSYMBOL、$DKANA、<br>$DHIRA、$DKANJI |
| $KANJI | 944 |Full-width characters other than full-width symbols, full-width / half-width spaces |Applicable to $DNUMERIC、$DALPHA、$DKANA、$DHIRA、$DKANJI |
| $EXSPACE | 0x40000000 | This is an option to add to the above specifications. Specify the exclusion of half-width spaces.<br>There is no effect even if it is specified in combination with $STD or alone.<br>**<small>More added since Version 5.0.3</small>** | Example) $DKANA+$EXSPACE<br>Only full-width katakana and double-byte spaces can be entered|
 
The function of the OS is used to judge the character type.
Different judgments may be made depending on the OS.
The characters "々" may be judged as symbols or Chinese characters by the OS, so be sure to check that they are judged correctly by the OS you actually use.