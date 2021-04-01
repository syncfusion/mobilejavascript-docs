---
layout: post
title: data-binding
description: data binding
platform: js
control: ListView
documentation: ug
---

# Data binding

## Local data binding

The local data can be an array of JSON objects which is assigned for the ListView widget’s datasource property. Refer the below example.

{% highlight html %}

<ul data-role="ejmlistview" id="locallistbox" data-ej-datasource="window.dbitem" data-ej-fields-text="text"></ul>


{% endhighlight %}



{% highlight js %}

window.dbitem = [{ "text": "Discover Music" },
            { "text": "Sales and Events" },
            { "text": "Categories" },
            { "text": "MP3 Albums" },
            { "text": "More in Music" }];


{% endhighlight %}

![](data-binding_images\data-binding_img1.png)

## Remote data binding

The ListView control also provides support for Remote data binding. Here the remote data is placed in Web service and you can render the list items from the web service using Service URL. The data is in JSONformat.

{% highlight html %}

<ul data-role="ejmlistview" id="remotelistbox" data-ej-datasource="window.datasource" data-ej-fields-text="ShipCity" data-ej-itemscount="10">
            </ul>


{% endhighlight %}



{% highlight js %}

window.datasource = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Orders"
        });


{% endhighlight %}

![](data-binding_images\data-binding_img2.png)

