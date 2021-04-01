---
layout: post
title: Customize Values | Rating | Mobilejs | Syncfusion
description: customize values
platform: Mobilejs
control: Rating (Mobile)
documentation: ug
keywords: rating, value, minvalue, maxvalue
---

# Customize values

The "data-ej-maxvalue" attribute is used to denote the maximum value up to which the rating can be accepted. The data-ej-minvalue attribute is used to denote the minimum rating value. The "data-ej-value" attribute specifies the current selection value. The "data-ej-incrementstep" attribute specifies the step value incrementation between each rating value (star) selection.

{% highlight html %}

<div id="rating_sample" data-role="ejmrating" data-ej-minvalue=2 data-ej-maxvalue=6 data-ej-value=4 data-ej-incrementstep=1>

</div>

{% endhighlight %}

The following screenshot displays the output.

![](Customize-Values_images/Customize-Values_img1.png)