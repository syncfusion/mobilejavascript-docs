---
layout: post
title: Data Binding | DropDownList | Mobilejs | Syncfusion
description: data binding
platform: Mobilejs
control: DropDownList (Mobile)
documentation: ug
keywords : selection 
---

# Selection

## Multiple selection

DropDownList has a check list feature that is used to select multiple list items, by using set enableMultiSelect property as true.

{% highlight html %}

    <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData"
            data-ej-watermarktext="Select a Country" data-ej-fields-text="name" data-ej-enablemultiselect="true"/>

{% endhighlight %}

To include datasource, add the following script.

{% highlight js %}

        window.listData = [{ name: "Australia"},
                           { name: "Brazil" },
                           { name: "China" },
                           { name: "India"},
                           { name: "Spain" },
                           { name: "United States of America" }
        ];

{% endhighlight %}

The following screenshot displays the Local Data Binding:

![](Selection-images/Selection-img1.png)

