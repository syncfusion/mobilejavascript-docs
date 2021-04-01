---
layout: post
title: selection
description: selection
platform: js
control: ListView
documentation: ug
---

# Selection

## Multiple Selection

ListView has a check list feature that is used to select multiple list items, by using set EnableCheckList property as true.

{% highlight html %}


    <ul id="lb" data-role="ejmlistview" data-ej-enablechecklist="true">
        <li data-ej-text="Artwork"></li>
        <li data-ej-text="Abstract"></li>
        <li data-ej-text="2 Acrylic Mediums"></li>
        <li data-ej-text="Creative Acrylic"></li>
        <li data-ej-text="Modern Painting"></li>
        <li data-ej-text="Canvas Art"></li>
        <li data-ej-text="Black white"></li>
        <li data-ej-text="Children"></li>
        <li data-ej-text="Preschool Crafts"></li>
        <li data-ej-text="School-age Crafts"></li>
    </ul>



{% endhighlight %}



The following screenshot displays Multiselection:

![](selection_images\selection_img1.png)

## Allow selection

When a specific list item is selected, it is highlighted with an active color. AllowSelection property prevents this behavior when set to true. 

{% highlight html %}


    <ul id="lb" data-role="ejmlistview" data-ej-allowselection="false">
        <li data-ej-text="Artwork"></li>
        <li data-ej-text="Abstract"></li>
        <li data-ej-text="2 Acrylic Mediums"></li>
        <li data-ej-text="Creative Acrylic"></li>
        <li data-ej-text="Modern Painting"></li>
        <li data-ej-text="Canvas Art"></li>
        <li data-ej-text="Black white"></li>
        <li data-ej-text="Children"></li>
        <li data-ej-text="Preschool Crafts"></li>
        <li data-ej-text="School-age Crafts"></li>
    </ul>


{% endhighlight %}



## Persist selection

PersistSelection property is used to highlight the selected item in the ListView control even after touch end happens. By default, the active state is removed once touch end happens.

{% highlight html %}

    <ul id="lb" data-role="ejmlistview" data-ej-persistselection="true">
        <li data-ej-text="Artwork"></li>
        <li data-ej-text="Abstract"></li>
        <li data-ej-text="2 Acrylic Mediums"></li>
        <li data-ej-text="Creative Acrylic"></li>
        <li data-ej-text="Modern Painting"></li>
        <li data-ej-text="Canvas Art"></li>
        <li data-ej-text="Black white"></li>
        <li data-ej-text="Children"></li>
        <li data-ej-text="Preschool Crafts"></li>
        <li data-ej-text="School-age Crafts"></li>
    </ul>


{% endhighlight %}



![](selection_images\selection_img2.png)

