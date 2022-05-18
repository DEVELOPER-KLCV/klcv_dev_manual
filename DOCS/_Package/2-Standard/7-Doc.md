---
layout: default

parent: 2. Standard Package
has_children: true

title: Doc Class
nav_order: 7
permalink: /package/standard/doc

---

# {{ page.title }}

<a href="/img/Package/Standard-Doc.PNG" target="blank"><img src="/img/Package/Standard-Doc.PNG" alt="Standard-Doc"></a>

This class has a function to output to a printer.<br>

Outputs the screen display class object placed under the Doc object to the printer.<br><br>

 

The Doc object corresponds to the output printing paper itself. Specify the paper and output printer for each property of the Doc class.<br><br>

 

The printing behavior of the placed display object depends on the implementation of each class. Some classes are not printed even if they are placed. See the description of each class for details.

**Default properties and ValueType**
The default property is <a href="/package/standard/doc/properties/value">Value</a>. ValueType can be String , Number , Fixed , or Date.

**Example of use**

```
Doc Doc1 {
    Format = "A4H";
    Form Form1 {
        Width = 400;
        Height = 400;
        Label Label1 {
            Width = 80;
            Height = 30;
            Border = $ TRUE;
        }
    }
    ShowPage ();
    Delete ();
}
```

**Preview Screen** <br>

{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

Specify $ SCREEN for the <a href="/package/standard/doc/properties/preview">Preview</a> property to display the preview screen. On the preview screen, you can check the print result before printing.

When debugging with Biz / Desiger, the preview screen is always displayed regardless of the property specified.

**Delete Doc object**<br>
The print job is completed when the Doc object is deleted by the  <a href="/system/object/methods/delete">Delete</a> method. After printing the last page (or a single page) with the <a href="/package/standard/doc/methods/showpage">ShowPage</a> method, be sure to call the Delete method to delete the Doc object.

**Differences from Biz / Designer's design view**<br>
There is a difference between the display of Doc objects in the design view of Biz / Designer and the actual printing and preview display. This is due to the difference in resolution between the screen and the printer and the operation of page break control. Adjust the print layout after actually checking the preview and print results.

**Restrictions when visual style is enabled**<br>
◆ Specifying the visual style is invalid.

**Precautions when scaling**<br>
Nothing in particular.

