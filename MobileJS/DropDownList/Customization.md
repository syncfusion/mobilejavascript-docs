---
layout: post
title: Data Binding | DropDownList | Mobilejs | Syncfusion
description: data binding
platform: Mobilejs
control: DropDownList (Mobile)
documentation: ug
keywords : watermark , height , width
---

# Customization

## Adding watermark text

It provides the short description of the expected value in dropdown and will display the text until any item is selected. You can set this text using data-ej-watermarktext attribute.

{% highlight html %}

 <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData"
            data-ej-watermarktext="Select a Country" data-ej-fields-text="name"/>

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

![](Customization-images/Customization-img1.png)

## Height and width customization

You can customize the DropDownList by using data-ej-popupwidth and data-ej-popupheight attributes.

{% highlight html %}

  <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData"
            data-ej-watermarktext="Select a Country" data-ej-fields-text="name" data-ej-popupheight="200px" data-ej-popupwidth="200px"/>

</div>

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

The following screenshot displays the height and width customization of DropDownList.

![](Customization-images/Customization-img2.png)

