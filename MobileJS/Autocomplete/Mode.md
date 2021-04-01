---
layout: post
title: mode
description: mode
platform: js
control: Overview
documentation: ug
---

## Mode

The data-ej-mode attribute specifies the textbox type. The possible values are,

1. Default

2. Search

Default is used to render the Autocomplete as normal textbox. Search is used to render the control with search icon. Default value for the attribute is “default”.

{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-mode="search" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



![](mode_images\mode_img1.png)

