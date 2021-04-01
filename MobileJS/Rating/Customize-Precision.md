---
layout: post
title: Customize Precision | Rating | Mobilejs | Syncfusion
description: customize precision
platform: Mobilejs
control: Rating (Mobile)
documentation: ug
keywords: rating, precision
---

# Customize precision

The data-ej-precision attribute is used to specify how the Rating control can accept its value. The possible values are,

1. Full Precision-accepts rounded value based on the selection.
2. Exact Precision-accepts exact selected value.
3. Half Precision-accepts exact half/rounded value based on the selection (0.5, 1, 1.5, 2, etc.).

{% highlight html %}

<div id="rating_sample" data-role="ejmrating" data-ej-precision="exact">

</div> 

{% endhighlight %}

The following screenshot displays the output.                        

![](Customize-Precision_images/Customize-Precision_img1.png)