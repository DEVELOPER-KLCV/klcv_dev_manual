---
layout: default

parent: 1. System Package
has_children: true

title: RegexPattern Class
nav_order: 13
permalink: /package/system/regexpattern

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

A class that holds regular expression patterns.

The [Compile]() static method compiles the specified regular expression and creates a RegexPattern object.
The generated RegexPattern object is used to generate an object of the [RegexMatcher]() class, which is a regular expression engine for matching with any input string.

You can create multiple RegexMathcer objects from a single RegexPattern object. Each RegexMatcher object shares the same regular expression pattern.

<b>Default properties and ValueType</b>

The default property is [Pattern](). The ValueType specification is invalid.

**<small>A Unicode mode has been added that handles more Unicode strings. -></small>**

<b>About Unicode mode</b>

If you specify RegexPattern.Unicode as an argument of [Compile]() method and [Matches]() method, you can generate a regular expression engine in Unicode mode.

In Unicode mode, regular expressions and input strings are treated as UString type, and Unicode characters can be used.

The index that represents the position of the character ([Start]() of RegexMatcher class, result of [End]() method, etc.) is in character units (byte units when not in Unicode mode).

**<small><-Up to here</small>**

<b>Typical usage</b>

<ol>
    <li>Compile the regular expression with the Compile static method to create a RegexPattern object.</li>
    <li>Create a RegexMatcher object that matches the regular expression pattern and the input string by the Matcher method of the RegexPattern object generated in 1.</li>
    <li>Match with the Matches method, Find method, etc. of the RegexMatcher object generated in 2.</li>
</ol>

```
/* 正規表現をコンパイルします */
var p = RegexPattern.Compile("Biz/([a-zA-Z]+)");
/* 入力文字列を設定し正規表現エンジンを生成します */
var m = p.Matcher("Biz/Browser, Biz/Designer");
 
/* 部分一致検索を行います */
while (m.Find()) {
    /* 部分一致した部分全体を表示 */
    print(m.Group());
    /* 一つ目の前方参照グループを表示 */
    print(" [", m.Group(1) , "]", "\n");
}
/* 全体完全一致 */
print("Matches:", m.Matches(), "\n");
 
/* 先頭からのマッチ */
print("LookingAt:", m.LookingAt(), "\n");
 
----- 実行結果 -----
Biz/Browser [ Browser ]
Biz/Designer [ Designer ]
Matches: 0
LookingAt: 1
```

<u><b>Regular expression syntax summary</b></u>
 
You can use Perl-like syntax for regular expressions.
* PCRE (Perl Compatible Regular Expressions) is used in the regular expression class.

<b>Metacharacters</b>

<table>
    <tr>
        <td>\</td>
        <td>Quote the meta character immediately after</td>
    </tr>
    <tr>
        <td>^</td>
        <td>Matches the beginning of a line. The beginning of a line in multi-line mode.</td>
    </tr>
    <tr>
        <td>.</td>
        <td>Matches any character (except line breaks).</td>
    </tr>
    <tr>
        <td>$</td>
        <td>Matches the end of a line. End of line in multi-line mode.</td>
    </tr>
    <tr>
        <td>|</td>
        <td>Selection</td>
    </tr>
    <tr>
        <td>()</td>
        <td>Grouping</td>
    </tr>
    <tr>
        <td>[]</td>
        <td>Character class</td>
    </tr>
</table>

<b>Metacharacters that can be used in character classes</b>

| \ | Quote the meta character immediately after |
| ^ | Negate the class only when used for the first character |
| - | Character range ※ |

※ The regular expression of Biz / Browser uses UTF-8 as the character code of the internal data. When specifying the character range, the UTF-8 character code is used to determine the range. (It is always UTF-8 regardless of the Unicode mode specification.) Be careful when specifying characters such as "Kanji" in the range.

<b>Binary character</b>

| \t | Tab |
| \n | New line |
| \r | Return |
| \f | New page |
| \a | Alarm (bell) | 
| \e | Escape |
| \033 | Eighth character |
| \x1B | Hexadecimal character |
| \c[ | Control character |
| \E | Ends quoting of regular expression operators started with \Q |
| \Q | Treats all special characters up to \E as normal characters |

<b>General character</b>

| \w | Matches "word" characters (alphabets, numbers, "_") |
| \W | Matches non-word characters |
| \s | Matches whitespace characters |
| \S | Matches non-blank characters |
| \d | Matches numbers |
| \D | Matches non-numbers |

<b>Position specifier</b>

| \b | Matches word boundaries |
| \B | Matches other than word boundaries |
| \A | Matches only at the beginning of the string |
| \Z | Matches only at the end of the string or just before the newline at the end |
| \z | Matches only at the end of the string |
| \G | Matches the search start position |

<b>Character class[:class:]</b>

| alnum | alphanumeric |
| alpha | english alphabet   |
| ascii | character code 0 - 127   |
| blank | Blank or tab   |
| cntrl | Control character   |
| digit | 10-decimal digits   |
| graph | Excluding displayable character spaces |
| lower | Lowercase letters |
| print | Indicates possible text |
| punct | Punctuation characters |
| space | Space characters |
| upper | Uppercase characters |
| word  | Matches "word" characters (alphabets, numbers, "_")|
| xdigit | 16 digits |

<b>Quantum specifier</b>

|*  |Matches zero or more iterations|
|+  |Matches more than once|
|?  |Matches zero or one iteration|
|{n}    |Matches n iterations|
|{n,}   |Matches at least n repeats|
|{n,m}  |Matches repeats between n and m times|
