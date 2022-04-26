---
layout: default

grand_parent: Root Class
parent: Methods
has_children: false
title: Root.SetMenu Property
nav_order: 24
permalink: /package/standard/root/methods/setmenu
---
# {{ page.title }}

<table>
  <tr>
    <td>Explanation</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td>Call format</td>
    <td colspan="2">//.SetMenu( [ <b>menuXML</b> ] )</td>
  </tr>
  <tr>
    <td>Return value</td>
    <td colspan="2">None</td>
  </tr>  
  <tr>
    <td>Arguments</td>
    <td>XMLDocument <b>menuXML</b></td>
    <td></td>
  </tr>
  <tr>
    <td>Exception</td>
    <td colspan="2">None</td>
  </tr>
  <tr>
    <td>Example of use</td>
    <td colspan="2">
    <code><pre>
    var x = new XmlDocument();
x << xml <<-
    &lt;?xml version="1.0" encoding="SHIFT_JIS"?&gt;
    &lt;menudefine&gt;
        &lt;menu title="ファイル"&gt;
            &lt;menuitem id="11" title="トップ" /&gt;
            &lt;separator /&gt;
            &lt;menuitem id="18" title="設定" /&gt;
            &lt;menuitem id="19" title="終了" /&gt;
        &lt;/menu&gt;
        &lt;menu title="業務"&gt;
            &lt;menuitem id="31" title="日報入力" /&gt;
            &lt;menuitem id="32" title="出勤入力" /&gt;
            &lt;menuitem id="33" title="販売管理" /&gt;
        &lt;/menu&gt;
        &lt;menu title="マスタ管理"&gt;
            &lt;menuitem id="91" title="ユーザー情報"&gt;
            &lt;/menuitem&gt;
        &lt;/menu&gt;
    &lt;/menudefine&gt;
->>;
//.SetMenu(x);
    </pre></code></td>
  </tr>
  <tr>
    <td>Related item</td>
    <td colspan="2"><a href="/package/standard/root/events/menuselected">MenuSelected</a> event<br><a href="">XmlDocument</a> class</td>
  </tr>
</table>


<b>Menu definition XML format</b>




