---
layout: post
title: Customize value | Numeric Textbox | Mobilejs | Syncfusion
description: customize value
platform: Mobilejs
control: Numeric Textbox (Mobile)
documentation: ug
keywords: value
---

# Customize value

The current value of the Numeric Textbox can be specified by using the Value property. The range for the Numeric Textbox can be specified by using the MaxValue and MinValue properties. The Numeric Textbox can only accept values within those specified range. The step property is used to set the step value in each incrementing or decrementing textbox when the spin buttons are clicked or up/down arrows are used.

{% highlight html %}

<input id="sample" name="sample" data-role="ejmnumeric" type="number"  data-ej-value="30" data-ej-step="2" data-ej-maxvalue="100" data-ej-minvalue="20"  />

{% endhighlight %}

The following screenshot displays the output.

![](Customize-value_images/Customize-value_img1.png)

The DecimalPlaces property makes you restrict the decimal places to set the decimal (floating point) numbers.

{% highlight html %}

<input type="number" id="textbox_sample" data-role="ejmnumeric" data-ej-decimalPlaces="3"/>

{% endhighlight %}