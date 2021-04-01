---
layout: post
title: multi-selection
description: multi selection
platform: js
control: Overview
documentation: ug
---


## Multi value selection

Autocomplete textbox enables you to select multiple items from the suggestion list. To achieve this, set the data-ej-enablemultiselect attribute to true. The data-ej-delimiterchar attribute holds a string value that specifies the separator between two selected items. You can customize the delimiter string. In this example “;” is used as delimiter.

{% highlight html %}


<label>Select Contacts</label>
     <!-- Autocomplete control -->
<input id="contacts" data-role="ejmautocomplete" data-ej-watermarktext="Search Contacts" data-ej-datasource="window.contacts" data-ej-fields-text ="name" data-ej-enablemultiselect=true data-ej-delimiterchar=";"/>


{% endhighlight %}



![](multi-selection_images\multi-value-selection_img1.png)


## DelimiterChar

The data-ej-delimiterchar is used to separate two or more items in the Autocomplete textbox. If you set data-ej-delimiterchar attribute, the selected value gets added in the textbox only after the delimiter character is placed. Default value is “,”.


{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete"  data-ej-enablemultiselect="true" data-ej-delimiterchar=";" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight js %}

        window.datasrc = [
{ 'name': 'Audi S6' },
{ 'name': 'Audi S7' },
{ 'name': 'BMW 7' },
{ 'name': 'Chevrolet Camaro' },
{ 'name': 'Duesenberg J' },
{ 'name': 'Elantra' }
];


{% endhighlight %}




![](multi-selection_images\delimiterchar_img1.png)