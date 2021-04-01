---
layout: post
title: data-binding
description: data binding
platform: js
control: Rotator (Mobile)
documentation: ug
---

## Data binding

The Essential JavaScript Mobile Rotator provides support for data binding. Data binding provides a simple and consistent way for applications to present and interact with data. Elements can be bound to data from a variety of data sources.

data-ej-datasource is used to get the datasource that holds the Rotator items. Refer to the following code example.

{% highlight html %}

  <div class="sample-control databinding rotator page">
        <div id="databindrotator" data-role="ejmrotator" data-ej-targetid="rotatorcontentdatabinding" data-ej-datasource="window.imgdata">
        </div>
    </div>
    <div id="rotatorcontentdatabinding">
        <div class="e-m-rotator-image {{:imageurl}}">
        </div>
    </div>


{% endhighlight %}



Refer the below code snippets for script section

{% highlight js %}

  window.imgdata = [
            {
                imageurl: "image-bread",
            },
            {
                imageurl: "image-card",
            },
            {
                imageurl: "image-green",
            },
            {
                imageurl: "image-tablet",
            },
            {
                imageurl: "image-wheat",
            }
        ];	


{% endhighlight %}

![](data-binding_images\data-binding_img1.png)

