---
layout: default

grand_parent: 4. Extension4 Package
parent: StyleEdit Class

title: Properties
nav_order: 1
permalink: /package/extension4/styleedit/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the StyleEdit class.

|Name       | Access | Type   | Initial Value | Description   |
|----------	|--------|--------|---------------|---------|
|[AcceptDrop](/package/extension4/styleedit/properties/acceptdrop) | CR | integer | 0 |Type that accepts drag and drop |
|[Anchor](/package/extension4/styleedit/properties/anchor) | CRW | integer | 0 |Current anchor position |
|[AutoIndent](/package/extension4/styleedit/properties/autoindent) | CRW | boolean | $FALSE |ON/OFF of auto indent |
|[Border](/package/extension4/styleedit/properties/autoindent) | CRW | boolean | $FALSE |Frame display |
|[CaretLine](/package/extension4/styleedit/properties/caretline) | CRW | boolean | $FALSE |Display the cullet line indicator |
|[CaretLineColor](/package/extension4/styleedit/properties/caretlinecolor) | CRW | integer | $STD |Caret line indicator color | 
|[FoldBrace](/package/extension4/styleedit/properties/foldbrace) | CRW | boolean | $FALSE |ON / OFF of folding function between braces<br><small><span style="color:red">Added since Ver.4.1.3</span></small> | 
|[FontFace](/package/extension4/styleedit/properties/fontface) | CRW | integer | $STD |Font decoration attributes | 
|[FontKind](/package/extension4/styleedit/properties/fontkind) | CRW | integer | $STD |Font type | 
|[FontSize](/package/extension4/styleedit/properties/fontsize) | CRW | integer | 10 |Font size | 
|[LineNumber](/package/extension4/styleedit/properties/linenumber) | CRW | boolean | $FALSE |ON / OFF of line number display | 
|[LineWidthLimit](/package/extension4/styleedit/properties/linewidthlimit) | CRW | integer | 0 | Maximum line width for automatic line breaks<br><small><span style="color:red">Added since Ver.4.2.0</span></small>| 
|[Position](/package/extension4/styleedit/properties/position) | CRW | integer | 0 |Current cullet position | 
|[ShowCaret](/package/extension4/styleedit/properties/showcaret) | CR | boolean | $TRUE |Invalid. The specification is ignored. | 
|[TabSize](/package/extension4/styleedit/properties/tabsize) | CRW | integer | 4 |Tab width | 
|[UseContextMenu](/package/extension4/styleedit/properties/usecontextmenu) | CRW | boolean | $TRUE |Whether to use the context menu <br><small><span style="color:red">Added since Ver.4.1.3</span></small> | 
|[UseTabs](/package/extension4/styleedit/properties/usetabs) | CRW | boolean | $TRUE |Whether to use tab characters | 
|[Value](/package/extension4/styleedit/properties/value)* | CRW | String |  |Entered value | 
|[ViewEOL](/package/extension4/styleedit/properties/vieweol) | CRW | boolean | $FALSE |ON / OFF of line feed symbol display | 
|[ViewWhiteSpace](/package/extension4/styleedit/properties/viewwhitespace) | CRW | boolean | $FALSE |ON / OFF of display of blank characters | 
|[WordWrap](/package/extension4/styleedit/properties/wordwrap) | CRW | boolean | $TRUE | Word wrap control| 
|[WordWrapMode](/package/extension4/styleedit/properties/wordwrapmode) | CRW | integer | $WORD |Rule for determining automatic line feed position<br><small><span style="color:red">Added since Ver.4.2.0</span></small> | 

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property