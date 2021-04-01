---
layout: post
title: autofill
description: autofill
platform: js
control: Overview
documentation: ug
---

## AutoFill

The data-ej-enableautofill attribute is used to automatically fill the Autocomplete textbox with the first suggestion result, when you enter the query. It matches the users query with the available suggestions and displays in the textbox as you type the phrase. By default, the value is set to “false”.

{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-enableautofill=true data-ej-datasource="window.datasrc" data-ej-filtertype="startswith" data-ej-fields-text="name" />


{% endhighlight %}




![](AutoFill_images\autofill_img1.png)

