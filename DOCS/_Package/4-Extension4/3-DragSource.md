---
layout: default

parent: 4. Extension4 Package
has_children: true

title: DragSource Class
nav_order: 3
permalink: /package/extension4/dragsource

---
{% assign img1 = "/img/Biz Browser V/Package_Button.png" %}


# {{ page.title }}
<br>

<a href="/img/Package/Ext4-DragSource.PNG" target="_blank">
<img src="/img/Package/Ext4-DragSource.PNG" alt="login image"></a>

A class for implementing drag and drop operations.

It can handle three types of data formats, and one DragSource object can be set and transferred at the same time.

1. It is possible to communicate with editors that support drag and drop in the standard Windows text transfer format (CF_TEXT format).

2. It is possible to communicate with a filer such as Explorer using the standard Windows file transfer format (CF_HDROP format).

3. It is possible to pass an object to another object in a reference format in the Biz / Browser original format. 

As a normal usage, you can create a DragSource object with an event handler such as the <a href="/package/extension4/trayicon/events/clicked">Clicked</a> event and take over to the drag and drop operation.

**Default properties and ValueType**<br>
There are no default properties. The ValueType specification is invalid.

Example of use

```
Label lbl_title {
    Value = "Test";
 
    Function OnClicked( e ) {
        var rec = new Record {
            Number num;
            String str;
        }
        var ds = new DragSource;
        ds.AddFile("C:\\test1.txt");
        ds.AddFile("D:\\test2.txt");
        ds.SetString(Value);
        ds.SetObject(rec);
        ds.DoDragDrop();
    }
}
```

