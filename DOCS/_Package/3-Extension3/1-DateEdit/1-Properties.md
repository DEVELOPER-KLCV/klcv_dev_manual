---
layout: default

grand_parent: 3. Extension3 Package
parent: DateEdit Class

title: Properties
nav_order: 1
permalink: /package/extension3/dateedit/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the DateEdit class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AutoTab](/package/extension3/dateedit/properties/autotab) | CRW | boolean | $FALSE |Automatically move focus by entering all digits <br><small><span style="color:green">Can be specified since Ver.4.0.0, Mobile Ver.2.0.0</span></small>|
|[Border](/package/extension3/dateedit/properties/border) | CR | boolean | $TRUE | Frame display |
|[DisableHelper](/package/extension3/dateedit/properties/disablehelper) | CRW | boolean | $FALSE |Disable calendar display<br><small><span style="color:red">Added since Ver.4.1.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[DisableToday](/package/extension3/dateedit/properties/disabletoday) | CRW | boolean | $FALSE | Disable today's date entry by double-clicking <br><small><span style="color:red">Added since Ver.4.2.0</span></small><br><small><span style="color:blue">Not supported in Mobile</span></small>|
|[EditText](/package/extension3/dateedit/properties/edittext) | CR | String |  | The character string displayed on the screen<br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[Format](/package/extension3/dateedit/properties/format) | CR | String |  | Format string<br><small><span style="color:green">Formats that can be specified since Ver.4.1.0, Mobile Ver.3.0.0 have been added.</span></small>|
|[HorizontalAlign](/package/extension3/dateedit/properties/horizontalalign) | CR | integer | $STD | Horizontal alignment|
|[InvalidDate](/package/extension3/dateedit/properties/invaliddate) | R | boolean | $FALSE | Check invalid dates|
|[ShowFormat](/package/extension3/dateedit/properties/showformat) | CR | boolean | $FALSE |Display the specified contents of the Format property<br><small><span style="color:red">Added since Ver.4.0.3, Mobile Ver.2.0.0</span></small> |
|[UndecidedStyle](/package/extension3/dateedit/properties/undecidedstyle) | CR | integer | $STD | Behavior when an invalid value is entered|
|[Value](/package/extension3/dateedit/properties/value)* | CRW | Date |  |The value to display in the DateEdit object<br><small><span style="color:green">The Value value is now automatically corrected according to the Format.</span></small> |
|[VerticalAlign](/package/extension3/dateedit/properties/verticalalign) | CR | integer | $STD | Vertical alignment (printing only)<br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
