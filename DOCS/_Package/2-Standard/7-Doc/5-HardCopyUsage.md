---
layout: default

grand_parent: 2. Standard Package
parent: Doc Class

title: Hard Copy Usage
nav_order: 5
permalink: /package/standard/doc/hardcopy

---


# {{ page.title }}

It is a method to print the object placed on the screen as it is as a hard copy (screen capture).

 

* If a class that cannot be printed is included, it will not be an accurate hard copy.

* Manually entered data will not be printed unless it is set in a script, so it will not be an accurate hard copy.


{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21e1-2.files/image001.png" %}

<a href="{{ img1 }}" target="_blank"> <img src="{{ img1 }}" alt="{{img1}}"></a>

```
<Form1.crs>

Form Form1 {
    ...
    Button Button1 {
        Title = "印刷";
        Function OnTouch(e) {
            /* Doc1.crsの呼び出し */
            Get("Doc1.crs");
            /* １頁目の印刷 */
            Doc1.ShowPage();
            /* Doc1の削除 */
            Doc1.Delete();
        }
    }
}

```

{% assign img2 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/pac/std/std21e1-2.files/image002.png" %}

<a href="{{ img2 }}" target="_blank"> <img src="{{ img2 }}" alt="{{img2}}"></a>

```
<Doc1.crs>

Doc Doc1 {
    Format = "A4H";
    /* Form1.crs を読み込む */
    Get("Form1.crs");
    /* 必要に応じてSpread、TextBoxに値をセットする */
    /* Form1.TextBox1に手入力されたデータを印刷したい場合は何らかの方法で取得する必要が有る */
    if (!$DESIGNTIME) {
        /* Doc1の高さをForm1と合わせる */
        Height = Form1.Height;
        /* Doc1の幅をForm1と合わせる */
        Width = Form1.Width;
    }
}
```
