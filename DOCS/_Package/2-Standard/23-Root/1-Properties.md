---
layout: default

grand_parent: 2. Standard Package
parent: Root Class

title: Properties
nav_order: 1
permalink: /package/standard/root/properties

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}


# {{ page.title }}

The following properties are defined in the Root class.

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AltKeyPriority](/package/standard/root/properties/altkeypriority) | CRW | integer | 0 | 	Priority of event occurrence by key input <br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[BgColor](/package/standard/root/properties/bgcolor) | CRW | integer | $STD |Background color |
|[CacheMode](/package/standard/root/properties/cachemode) | CRW | integer | Root.CacheNetwork |Selection of communication method to be cached <br><small><span style="color:blue">Not supported in Mobile</span></small>|
|[CloseBox](/package/standard/root/properties/closebox) | CRW | boolean | $TRUE | Root window close button active / inactive <br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[ControlBox](/package/standard/root/properties/controlbox) | CRW | boolean | $TRUE |Show or hide the title bar button of the root window <br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[DirectInput](/package/standard/root/properties/directinput) | CRW | boolean | $FALSE |Specifies how to handle keystroke events internally  <br><small><span style="color:red">Added since Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[Embedded](/package/standard/root/properties/embedded) | R | integer |  | Whether it works within Internet Explorer <br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[ExtConnection](/package/standard/root/properties/extconnection) | R | boolean |  |Whether IEConnect is communicating <br><small><span style="color:red">Added since Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[HttpTimeout](/package/standard/root/properties/httptimeout) | CRW | integer | 0 | Communication timeout value  <br><small><span style="color:red">Added since Ver.4.1.0, Mobile Ver.3.0.0</span></small>|
|[Icon](/package/standard/root/properties/icon) | CRW | integer | 0 | Root window title bar icon <br><small><span style="color:red">Added since Ver.4.1.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[Indicator](/package/standard/root/properties/indicator) | CRW | integer | Root.indAll | Display of the status indicator displayed at the bottom of the screen <br><small><span style="color:red">Added since Ver.5.0.2, Mobile Ver.4.0.0, AI Ver.1.0.1</span></small> |
|[InputTimeout](/package/standard/root/properties/inputtimeout) | CRW | integer | 120 |Input operation timeout time <br><small><span style="color:red">Added since Ver.4.1.4</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[MaximizeBox](/package/standard/root/properties/maximizebox) | CRW | boolean | $TRUE | Allow root window maximization <br><small><span style="color:red">Added since Ver.4.0.1</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[MinimizeBox](/package/standard/root/properties/minimizebox) | CRW<br>CR<br>**<small>Mobile</small>** | boolean | $TRUE |	Allow root window minimization  <br><small><span style="color:red">Added since Ver.4.0.1, Mobile Ver.4.5.0</span></small><br><small><span style="color:blue">Not supported in AI</span></small>|
|[ReSize](/package/standard/root/properties/resize) | CRW | integer | $TRUE |Allow root window resizing <br><small><span style="color:green">Parameters that can be specified have been added from Ver.5.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[ShellId](/package/standard/root/properties/shellid) | CRW | String |  |ID of IE Connect to connect <br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[Title](/package/standard/root/properties/title) | CRW | String |  |Root window title text |
|[TitleBar](/package/standard/root/properties/titlebar) | CRW | boolean | $TRUE | Show or hide the root window title bar <br><small><span style="color:red">Added since Ver.4.0.1, Mobile Ver.5.0.3</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small> |
|[Value](/package/standard/root/properties/value)* | CRW | String |  | Object value|
|[X](/package/standard/root/properties/x) | CRW | integer |  | Horizontal display position of root window <br><small><span style="color:green">It can be specified since Mobile Ver.4.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|
|[Y](/package/standard/root/properties/y) | CRW | integer |  | 	Vertical display position of root window <br><small><span style="color:green">It can be specified since Mobile Ver.4.0.0</span></small><br><small><span style="color:blue">Not supported in Mobile, AI</span></small>|

**<small>Visible property can be specified after Version 4.1.3</small>**

Only available for Mobile version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[AutoDial](/package/standard/root/properties/autodial) | CRW | integer | Root.Up+Root.Down  |    Automatic dial-up control <br><small><span style="color:red">Added since Mobile Ver.3.0.1</span></small>        |
|[DialEntry](/package/standard/root/properties/dialentry) | CRW | String |   |      Connection name for dial-up connection<br><small><span style="color:red">Added since Mobile Ver.3.2.1 </span></small>|
|[HttpRetryTime](/package/standard/root/properties/httpretrytime) | CRW | integer | 0  |Reconnect timeout on dial-up connection<br><small><span style="color:red">Added since Mobile Ver.4.0.0 </span></small>|
|[UseHttpPreconfig](/package/standard/root/properties/usehttppreconfig) | CRW | boolean | $TRUE  | Whether to use standard proxy settings for communication   <br><small><span style="color:red">Added since Mobile Ver.3.1.0 </span></small>          |

Only available for Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[ReloggedIn](/package/standard/root/properties/reloggedin) | R | boolean | $FALSE  |Whether the Biz / Browser AI process was killed by an external factor             |
|[ScrollBarSize](/package/standard/root/properties/scrollbarsize) | CR | integer |  16  | Specifies the scrollbar size for the entire application        |
|[BackKeyMode](/package/standard/root/properties/backkeymode) | CRW | integer | Root.ConfirmClose+Root.RaiseKeyDown  |Specifies the behavior when the "Back" button is pressed <br><small><span style="color:red">Added since AI Ver.1.0.2 </span></small>   |

Only available for both Mobile and Android version

|Name       | Access | Type   | Initial Value | Description |
|----------	|--------|--------|---------------|-------------|
|[DisplayOrient](/package/standard/root/properties/displayorient) | CRW | integer | Root.deg0<br>**<small>Root.UNSPECIFIED in AI</small>**  |       Screen rotation direction <br><small><span style="color:red">Added since Mobile Ver.3.1.0</span></small>      |

<u><b>Access</b></u><br>
R: Readable
W: Writable
C: Initializable

*: default property
