---
layout: post
title: databinding
description: databinding
platform: js
control: Overview
documentation: ug
---

## Databinding


### Local Databinding

The data-ej-datasource attribute is used to provide the suggestion list to the Autocomplete. The list of items are passed as an array and by using the data-ej-datasource attribute, Autocomplete retrieves the suggestion list. The data-ej-fields-text attribute is used to map the specific field name of the given DataSource to render the suggestion list when user type is in the textbox. You can refer to the following code example. Here “window.datasrc” refers to JSON data.

{% highlight html %}

<label>Select Cars</label>
<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



Add the Following script.

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



![](data-binding_images\local-databinding_img1.png)

### Remote Databinding

{% highlight html %}

<label>Contacts</label>
<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="ContactName"/>


{% endhighlight %}



{% highlight js %}

        window.datasrc = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Customers"
        });


{% endhighlight %}

![](data-binding_images\remote-databinding_img1.png)

