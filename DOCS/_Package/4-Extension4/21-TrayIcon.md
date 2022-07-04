---
layout: default

parent: 4. Extension4 Package
has_children: true

title: TrayIcon Class
nav_order: 21
permalink: /package/extension4/trayicon

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-TrayIcon.PNG" target="_blank">
<img src="/img/Package/Ext4-TrayIcon.PNG" alt="login image"></a>

This class is for handling the tray icon displayed on the Windows task bar.

By combining with the  <a href="/package/extension4/trayicon/properties/visible">Visible</a> property of the <a href="/package/standard/root">Root</a> class, it is possible to create an application that stores Biz / Browser in the task tray.

Mouse operations on the tray icon are notified as events, and by describing the corresponding processing, it is possible to implement returning to the window state or terminating the application.

The image for the icon can be specified with the <a href="/package/extension4/trayicon/methods/setimage">SetImage</a> and <a href="/package/extension4/trayicon/methods/seticon">SetIcon</a> methods. If not specified, the Biz / Browser application icon will be displayed as a substitute.

**Default properties and ValueType**<br>
The default property is <a href="/package/extension4/trayicon/properties/value">Value</a>. The value type specification is invalid.

**Usage Example**

```
Form Form1 {
    TrayIcon TrayIcon1 {
        Function OnClicked(e) {
            /* トレイアイコンを消してBiz/Browserを再表示 */
            Visible = $FALSE;
            //.Visible = $TRUE;
            //.SetWindowState($RESTORE + $FRONT);
        }
    }
}
Function OnWindowStateChanged(e) {
    /* Biz/Browserの最小化 */
    if (e.state == $MINIMIZE) {
        /* トレイアイコンを表示してウィンドウ表示を消す */
        Form1.TrayIcon1.Visible = $TRUE;
        Visible = $FALSE;
    }
}
```


