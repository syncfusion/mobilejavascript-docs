---
layout: post
title: grouped-list
description: grouped list
platform: js
control: ListView
documentation: ug
---

## Grouped list

Here, you can learn how ListView with items are grouped together using the grouplist feature in ListView.

{% highlight html %}

    <!--Add Header Element Here-->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Mailbox" data-ej-isrelative="true">
    </div>

    <!--Add Listview Element Here-->
    <ul data-role="ejmlistview" id="grouplistsamp">
        <span>Mailboxes</span>
        <!--Add Listview Images Here-->
        <li data-ej-text="Inbox"></li>
        <li data-ej-text="VIP"></li>
        <span>Labels</span>
        <li data-ej-text="Draft"></li>
        <li data-ej-text="Sent"></li>
        <li data-ej-text="Junk"></li>
        <li data-ej-text="Trash"></li>
        <li data-ej-text="All Mail"></li>
        <li data-ej-text="Mail"></li>
    </ul>


{% endhighlight %}

![](grouped-list_images\grouped-list_img1.png)

