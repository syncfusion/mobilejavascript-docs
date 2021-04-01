---
layout: post
title: customize-suggestion-list
description: customize suggestion list
platform: js
control: Overview
documentation: ug
---

## Customize suggestion list

### Items count

The data-ej-itemscount attribute specifies the number of items to be displayed in the suggestion list.

{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-itemscount=2 data-ej-datasource="window.datasrc" data-ej-fields-text="name" />         


{% endhighlight %}


### FilterType

The data-ej-filtertype attribute is used to filter and display the suggestion list based on your requirements. The possible values are, 

1. startswith

2. contains

By default, the value for the attribute is “contains”.

{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-filtertype="contains" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight js %}

        window.datasrc = [
{ 'name': 'Audi S6' },
{ 'name': 'Audi S7' },
    { 'name': 'Audi S8' },
{ 'name': 'BMW 7' },
{ 'name': 'Chevrolet Camaro' },
{ 'name': 'Duesenberg J' },
{ 'name': 'Elantra' }
        ];


{% endhighlight %}

![](Customize-suggestion-list_images\filtertype_img1.png)



### EnableDistinct

The data-ej-enabledistinct attribute is used to hide or show the duplicate items from the suggestion list. By default, the value for the attribute is “false”.

{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-enabledistinct="false" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight js %}

  window.datasrc = [
{ 'name': 'Audi S6' },
    { 'name': 'Audi S7' },
    { 'name': 'Audi S8' },
    { 'name': 'Audi S8' },
    { 'name': 'Audi S9' },
{ 'name': 'BMW 7' },
{ 'name': 'Chevrolet Camaro' },
{ 'name': 'Duesenberg J' },
{ 'name': 'Elantra' }
];


{% endhighlight %}

![](Customize-suggestion-list_images\enabledistinct_img1.png)



### Sorting 

The data-ej-allowsorting attribute enables the sorting operation for the suggestion list. When it is set to true, the suggestion list is displayed in the sorting order that can be given by using the “data-ej-sortorder” attribute.

The possible values are,

1. ascending

2. descending



{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-sortorder="descending" data-ej-allowsorting="true" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight js %}

    window.datasrc = [
{ 'name': 'Audi S6' },
    { 'name': 'Audi S7' },
    { 'name': 'Audi S8' },
    { 'name': 'Audi S8' },
    { 'name': 'Audi S9' },
{ 'name': 'BMW 7' },
{ 'name': 'Chevrolet Camaro' },
{ 'name': 'Duesenberg J' },
{ 'name': 'Elantra' }
];


{% endhighlight %}


![](Customize-suggestion-list_images\sorting-_img1.png)

### Empty Result

The data-ej-showemptyresulttext attribute is used to show or hide the suggestion box when there is no suggestion available for the user query. By default, the value is “true”.

The data-ej-emptyresulttext attribute is used to customize the text that is displayed when no results appear in the suggestion list. By default, the value is “No Suggestions”.



{% highlight html %}

<input id="autocomplete_sample" data-role="ejmautocomplete" data-ej-showemptyresulttext="true" data-ej-emptyresulttext="No Values available" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



![](Customize-suggestion-list_images\emptyresultempty-result_img1.png)

