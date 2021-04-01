---
layout: post
title: imagefield
description: imagefield
platform: js
control: Overview
documentation: ug
---

### ImageField

The data-ej-fields-image attribute is used to map the specific field name of the given DataSource to render the icons/images for each suggestion list. The mapped field should contain the icon/image URL for each suggestion list.

{% highlight html %}

<input id="ac_multivalue" data-role="ejmautocomplete" data-ej-enablemultiselect="true" data-ej-datasource="window.datasrc"
            data-ej-watermarktext="Select countries" data-ej-fields-text="country" data-ej-fields-image="flag" />


{% endhighlight %}



Add the following script.

{% highlight js %}

            window.datasrc = [
        {
            "country": "Afghanistan",
            "flag": "themes/sampleimages/countries/afghanistan.png"
        },
        {
            "country": "Bangladesh",
            "flag": "themes/sampleimages/countries/bangladesh.png"
        },
        {
            "country": "Canada",
            "flag": "themes/sampleimages/countries/Canada.png"
        }
            ];


{% endhighlight %}



![](imagefield_images\imagefield_img1.png)

