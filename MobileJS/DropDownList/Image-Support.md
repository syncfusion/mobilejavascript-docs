---
layout: post
title: Data Binding | DropDownList | Mobilejs | Syncfusion
description: data binding
platform: Mobilejs
control: DropDownList (Mobile)
documentation: ug
keywords : image
---

## Adding watermark text

You can add images to your DropDownList items by specifying the image class name for individual items using �data-ej-fields-image� attribute.

{% highlight html %}

<input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData"
            data-ej-watermarktext="Select nationality" data-ej-fields-text="name" data-ej-fields-image="image" />

{% endhighlight %}

To include datasource, add the following script.

{% highlight js %}

        window.listData = [{ name: "Australia", image: "themes/sampleimages/countries/Australia.png" },
                           { name: "Brazil", image: "themes/sampleimages/countries/Brazil.png" },
                           { name: "China", image: "themes/sampleimages/countries/china.png" },
                           { name: "India", image: "themes/sampleimages/countries/India.png" },
                           { name: "Spain", image: "themes/sampleimages/countries/Spain.png" },
                           { name: "United States of America", image: "themes/sampleimages/countries/Usa.png" }
        ];

{% endhighlight %}

The following screenshot displays the Local Data Binding:

![](Image-Support-images/Image-support_img1.png)

