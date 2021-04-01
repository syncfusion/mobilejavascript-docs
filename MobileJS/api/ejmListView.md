---
layout: post
title: ejmListView | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmListView
platform: Mobilejs
control: ejmListView
documentation: API
keywords: ejmListView, API, Essential Studio JS ListView (Mobile)
---

# ejmListView

The Essential JavaScript Mobile ListView widget builds interactive ListView interface. This control allows you to select an item from a list-like interface and display a set of data items in different layouts or views. Lists are used for displaying data, data navigation, result lists, and data entry.                                            

Custom Design for HTML ListView control.

$(element).ejmListView()



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview">
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





{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView();
    </script>



{% endhighlight %}





#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module: ej.globalize

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

## Members

### allowSelection `boolean`
{:#members:allowselection} 

Specifies whether the items are selectable or not.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-allowselection="false">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ allowSelection: false });
    </script>



{% endhighlight %}



### checkedIndices `numberarray`
{:#members:checkedindices} 

Specifies which items will be checked initially. This property works only for check list feature.

N> To use this property, enableChecklist property must be set as “true”.

#### Default Value

* []



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-enableChecklist="true" data-ej-checkedindices="[2,3]">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ enableChecklist: true, checkedIndices: [2, 3] });
    </script>



{% endhighlight %}


### cssClass `string`
{:#members:cssclass} 

Sets the root class for ListView. This cssClass API helps to use custom skinning option for ListView control. By defining the root class using this API, we need to include this root class in CSS.

Default Value

* ””

Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-cssclass="customclass">
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

    <style>
        .customclass .e-m-lv-content{
            color: red !important;
        }
    </style>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ cssClass: "customclass" });
    </script>

    <style>
        .customclass .e-m-lv-content{
            color: red !important;
        }
    </style>


{% endhighlight %}





### dataSource `jsonarray`
{:#members:datasource} 

Specifies the data source for ListView rendering. In Listview, ListView items can be given as datasource which consists of JSON array.

N> To render ListView with JSON array, the property fields.text should be set to map the ListView item's text.

#### Default Value

* []



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text"></ul>

    <script>
    window.dbitem =
    [{ "text": "Hot Singles" },
        { "text": "Rising Artists" },
        { "text": "Live Music" },
        { "text": "Best of 2013 So Far" },
        { "text": "100 Albums - $5 Each" },
        { "text": "Hip-Hop and R&amp;B Sale" },
        { "text": "CD Deals" }];
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script>
        window.dbitem =
        [{ "text": "Hot Singles" },
            { "text": "Rising Artists" },
            { "text": "Live Music" },
            { "text": "Best of 2013 So Far" },
            { "text": "100 Albums - $5 Each" },
            { "text": "Hip-Hop and R&amp;B Sale" },
            { "text": "CD Deals" }];

        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text" } });
    </script>


{% endhighlight %}



### deleteMode `enum`
{:#members:deletemode} 

This property enables delete option for each ListView item when swipe left happens to the ListView item. See [DeleteMode](http://help.syncfusion.com/mobilejs/api/global.html).

#### Default Value

* “none”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-deletemode="swipe">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ deleteMode: "swipe"});
    </script>



{% endhighlight %}



### enableChecklist `boolean`
{:#members:enablechecklist} 

Specifies whether to enable check mark for the item.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-enableChecklist="true">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ enableChecklist: true });
    </script>



{% endhighlight %}



### enabled `boolean`
{:#members:enabled} 

Specifies whether the control is enabled or disabled.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-enabled="false">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ enabled: false });
    </script>



{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence} 

Current model value to browser cookies for state maintains. While refresh the ListView control page retains the model value apply from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-enablepersistence="true">
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





{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ enablePersistence: true });
    </script>



{% endhighlight %}







### enableRippleEffect `boolean`
{:#members:enablerippleeffect} 

Specifies whether to enable or disable ripple effect.

#### Default Value

* ej.isAndroid() ? true : false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-enablerippleeffect="true">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ enableRippleEffect: true });
    </script>



{% endhighlight %}




### fields
{:#members:fields} 

Specifies the field settings to map the datasource.




### fields.allowSelection `boolean`
{:#members:fields-allowselection} 

Specifies whether the ListView individual item is selectable or not.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text" data-ej-fields-allowselection="selection"></ul>

    <script>
        window.dbitem =
            [{ "text": "Hot Singles", selection: false },
                { "text": "Rising Artists" },
                { "text": "Live Music", selection: false },
                { "text": "Best of 2013 So Far", selection: false },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>
    <script>
        window.dbitem =
            [{ "text": "Hot Singles", selection: false },
                { "text": "Rising Artists" },
                { "text": "Live Music", selection: false },
                { "text": "Best of 2013 So Far", selection: false },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];
    </script>

    <script>
        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text", allowSelection: "selection" } });
    </script>



{% endhighlight %}



### fields.badge `jsonobject`
{:#members:fields-badge} 

Maps badge field from the data source. Used to set value and maxValue for each item.

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text" data-ej-fields-badge-value="badgevalue" data-ej-fields-badge-maxvalue="badgemaxvalue"></ul>

    <script>
        window.dbitem =
            [{ "text": "Hot Singles", "badgevalue": 23 },
                { "text": "Rising Artists" },
                { "text": "Live Music", "badgevalue": 88 },
                { "text": "Best of 2013 So Far", "badgevalue": 123, "badgemaxvalue": 88 },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>
    <script>
        window.dbitem =
            [{ "text": "Hot Singles", "badgevalue": 23 },
                { "text": "Rising Artists" },
                { "text": "Live Music", "badgevalue": 88 },
                { "text": "Best of 2013 So Far", "badgevalue": 123, "badgemaxvalue": 88 },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];

        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text", badge: { value: "badgevalue", maxValue: "badgemaxvalue" } } });
    </script>



{% endhighlight %}



### fields.checkBy `string`
{:#members:fields-checkby} 

Maps the check status for each item in ListView initially. This is an optional property used only for check list.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-enablechecklist="true" data-ej-datasource="window.dbitem" data-ej-fields-text="text" data-ej-fields-checkby="check"></ul>

    <script>
    window.dbitem =
        [{ 'text': 'Hot Singles', 'check': true },
            { 'text': 'Rising Artists' },
            { 'text': 'Live Music', 'check': true },
            { 'text': 'Best of 2013 So Far', 'check': true },
            { 'text': '100 Albums - $5 Each' },
            { 'text': 'Hip-Hop and R&amp;B Sale' },
            { 'text': 'CD Deals' }];
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>
    <script>
        window.dbitem =
        [{ 'text': 'Hot Singles', 'check': true },
            { 'text': 'Rising Artists' },
            { 'text': 'Live Music', 'check': true },
            { 'text': 'Best of 2013 So Far', 'check': true },
            { 'text': '100 Albums - $5 Each' },
            { 'text': 'Hip-Hop and R&amp;B Sale' },
            { 'text': 'CD Deals' }];
    </script>

    <script>
        $("#listview").ejmListView({ enableCheckList: true, dataSource: window.dbitem, fields: { text: "text", checkBy: "check" } });
    </script>


{% endhighlight %}



### fields.enabled `boolean`
{:#members:fields-enabled} 

Maps enabled field from the data source. This property ensures whether the item is enabled or disabled initially.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text" data-ej-fields-enabled="enabled"></ul>

    <script>
        window.dbitem =
            [{ "text": "Hot Singles", enabled: false },
                { "text": "Rising Artists" },
                { "text": "Live Music", enabled: false },
                { "text": "Best of 2013 So Far", enabled: false },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];

    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>
    <script>
        window.dbitem =
            [{ "text": "Hot Singles", enabled: false },
                { "text": "Rising Artists" },
                { "text": "Live Music", enabled: false },
                { "text": "Best of 2013 So Far", enabled: false },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];

    </script>

    <script>
        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text", enabled: "enabled" } });
    </script>



{% endhighlight %}



### fields.groupBy `string`
{:#members:fields-groupby} 

Maps the group name in which each ListView item belongs to in ListView. This is an optional property used only for grouped list.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text" data-ej-fields-groupby="group"></ul>

    <script>
        window.dbitem =
        [{ "text": "Hot Singles", "group": "Likes" },
            { "text": "Rising Artists", "group": "Likes" },
            { "text": "Live Music", "group": "Likes" },
            { "text": "Best of 2013 So Far", "group": "Dislikes" },
            { "text": "100 Albums - $5 Each", "group": "Likes" },
            { "text": "Hip-Hop and R&amp;B Sale", "group": "Dislikes" },
            { "text": "CD Deals", "group": "Dislikes" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script>
        window.dbitem =
        [{ "text": "Hot Singles", "group": "Likes" },
            { "text": "Rising Artists", "group": "Likes" },
            { "text": "Live Music", "group": "Likes" },
            { "text": "Best of 2013 So Far", "group": "Dislikes" },
            { "text": "100 Albums - $5 Each", "group": "Likes" },
            { "text": "Hip-Hop and R&amp;B Sale", "group": "Dislikes" },
            { "text": "CD Deals", "group": "Dislikes" }];

        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text", groupBy: "group" } });
    </script>


{% endhighlight %}



### fields.href `string`
{:#members:fields-href} 

Maps href field from the data source. href is set to the navigation URL of each item.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text" data-ej-fields-href="href"></ul>

    <script>
        window.dbitem =
            [{ "text": "Hot Singles", href: "inner.html" },
                { "text": "Rising Artists" },
                { "text": "Live Music", href: "inner2.html" },
                { "text": "Best of 2013 So Far", href: "inner3.html" },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];

    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>
    <script>
        window.dbitem =
            [{ "text": "Hot Singles", href: "inner.html" },
                { "text": "Rising Artists" },
                { "text": "Live Music", href: "inner2.html" },
                { "text": "Best of 2013 So Far", href: "inner3.html" },
                { "text": "100 Albums - $5 Each" },
                { "text": "Hip-Hop and R&amp;B Sale" },
                { "text": "CD Deals" }];

    </script>

    <script>
        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text", href: "href" } });
    </script>



{% endhighlight %}



### fields.image `string`
{:#members:fields-image} 

Maps image field from the data source. Image given by the image will be rendered at the left of ListView item's text.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="text" data-ej-fields-image="image" ></ul>
    <script>
        window.listData = [{ text: "Australia", image: "Australia.png" },
                           { text: "Brazil", image: "Brazil.png" },
                           { text: "China", image: "china.png" },
                           { text: "India", image: "India.png" },
                           { text: "Spain", image: "Spain.png" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>
    <script>
        window.listData = [{ text: "Australia", image: "Australia.png" },
                           { text: "Brazil", image: "Brazil.png" },
                           { text: "China", image: "china.png" },
                           { text: "India", image: "India.png" },
                           { text: "Spain", image: "Spain.png" }];

        $("#listview").ejmListView({ dataSource: window.listData, fields: { text: "text", image: "image" } });
    </script>



{% endhighlight %}



### fields.text `string`
{:#members:fields-text} 

Maps text field from the data source. This is a required property while rendering the ListView from data source. 

N> Since field mapping depends on data source, the dataSource property must be set with a JSON data.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text"></ul>

    <script>
    window.dbitem =
    [{ "text": "Hot Singles" },
        { "text": "Rising Artists" },
        { "text": "Live Music" },
        { "text": "Best of 2013 So Far" },
        { "text": "100 Albums - $5 Each" },
        { "text": "Hip-Hop and R&amp;B Sale" },
        { "text": "CD Deals" }];
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script>
        window.dbitem =
        [{ "text": "Hot Singles" },
            { "text": "Rising Artists" },
            { "text": "Live Music" },
            { "text": "Best of 2013 So Far" },
            { "text": "100 Albums - $5 Each" },
            { "text": "Hip-Hop and R&amp;B Sale" },
            { "text": "CD Deals" }];

        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text" } });
    </script>


{% endhighlight %}



### fields.value `string`
{:#members:fields-value} 

Maps the value for each option from the data source. This is an optional property. 

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.dbitem" data-ej-fields-text="text" data-ej-fields-value="text"></ul>

    <script>
    window.dbitem =
    [{ "text": "Hot Singles" },
        { "text": "Rising Artists" },
        { "text": "Live Music" },
        { "text": "Best of 2013 So Far" },
        { "text": "100 Albums - $5 Each" },
        { "text": "Hip-Hop and R&amp;B Sale" },
        { "text": "CD Deals" }];
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script>
        window.dbitem =
        [{ "text": "Hot Singles" },
            { "text": "Rising Artists" },
            { "text": "Live Music" },
            { "text": "Best of 2013 So Far" },
            { "text": "100 Albums - $5 Each" },
            { "text": "Hip-Hop and R&amp;B Sale" },
            { "text": "CD Deals" }];

        $("#listview").ejmListView({ dataSource: window.dbitem, fields: { text: "text", value: "text" } });
    </script>


{% endhighlight %}



### itemsCount `number`
{:#members:itemscount} 

Specifies how many items need to render initially from remote data source. 

N> This property works based on remote data source, hence the dataSource and fields.text properties should be set properly while rendering.

#### Default Value

* 0

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="ContactName" data-ej-query="ej.Query()" data-ej-itemscount="8"></ul>

    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });

        $("#listview").ejmListView({ dataSource: window.listData, fields: { text: "ContactName" }, query: "ej.Query()", itemsCount: 8 });
    </script>


{% endhighlight %}



### items `jsonarray`
{:#members:items} 

Specifies the ListView items as an array of JSON objects.

#### Default Value

* []

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-items="[{ 'text': 'Hot Singles' }, { 'text': 'Rising Artists' }, { 'text': 'Live Music' }, { 'text': 'Best of 2013 So Far' }, { 'text': '100 Albums - $5 Each' }, { 'text': 'Hip-Hop and R&amp;B Sale' }, { 'text': 'CD Deals' }]"></ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script>
        $("#listview").ejmListView({ items: [{ 'text': 'Hot Singles' }, { 'text': 'Rising Artists' }, { 'text': 'Live Music' }, { 'text': 'Best of 2013 So Far' }, { 'text': '100 Albums - $5 Each' }, { 'text': 'Hip-Hop and R&amp;B Sale' }, { 'text': 'CD Deals' }] });
    </script>



{% endhighlight %}



### persistSelection `boolean`
{:#members:persistselection} 

Specifies whether to retain the selection of the ListView item.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-persistselection="true">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ persistSelection: true });
    </script>



{% endhighlight %}



### query `string`
{:#members:query} 

This property used to filter data from remote data source.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="ContactName" data-ej-query="ej.Query().take(10)"></ul>

    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });

        $("#listview").ejmListView({ dataSource: window.listData, fields: { text: "ContactName" }, query: "ej.Query().take(10)" });
    </script>


{% endhighlight %}



### renderMode `enum`
{:#members:rendermode} 

Specifies the rendering mode of the ListView control. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global.html)

#### Default Value

* auto

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-rendermode="android">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ renderMode: "android" });
    </script>



{% endhighlight %}



### selectedIndex `number`
{:#members:selectedindex} 

Specifies which item to be selected initially for the ListView.

N> To show the selected item as active, persistSelection property must be set as true.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-persistselection="true" data-ej-selectedindex="2">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ selectedIndex: 2, persistSelection: true  });
    </script>



{% endhighlight %}



### templateId `boolean`
{:#members:templateid} 

Specifies ID of the element contains template contents.

N> For ListView template rendering, jsrender.js script required.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-templateid="templatecontent">
    </ul>    

    <script id="templatecontent" type="text/x-jsrender">
        <div class="contentdiv">
            <span class="name">{{>Name}}</span> <span class="designation">{{>Designation}}</span>
        </div>
    </script>

    <script type="text/javascript">
        window.listData =
        [{ "Name": "Brooke", "Designation": "HR Assistant" },
        { "Name": "Claire", "Designation": "HR Manager" },
        { "Name": "Erik", "Designation": "Training Specialist" },
        { "Name": "Grace", "Designation": "Development Manager" },
        { "Name": "Jacob", "Designation": "Recruitment Manager" }];
    </script> 

    <style>
        .name {
            margin-left: 15px;
        }

        .designation {
            font-size: 13px;
            float: right;
            margin-right: 15px;
        }
    </style>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview"></ul>

    <script id="templatecontent" type="text/x-jsrender">
        <div class="contentdiv">
            <span class="name">{{>Name}}</span> <span class="designation">{{>Designation}}</span>
        </div>
    </script>

    <script type="text/javascript">
        window.listData =
        [{ "Name": "Brooke", "Designation": "HR Assistant" },
        { "Name": "Claire", "Designation": "HR Manager" },
        { "Name": "Erik", "Designation": "Training Specialist" },
        { "Name": "Grace", "Designation": "Development Manager" },
        { "Name": "Jacob", "Designation": "Recruitment Manager" }];

        $("#listview").ejmListView({ dataSource: window.listData, templateId: "templatecontent"  });

    </script> 

    <style>
        .name {
            margin-left: 15px;
        }

        .designation {
            font-size: 13px;
            float: right;
            margin-right: 15px;
        }
    </style>



{% endhighlight %}



### windows
{:#members:windows} 

Section for windows mode specific functionalities.

### windows.preventSkew `boolean`
{:#members:windows-preventskew} 

Specifies whether to prevent skewing behavior in windows mode.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-rendermode="windows" data-ej-windows-preventskew="true">
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



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ renderMode: "windows", windows: { preventSkew: true } });
    </script>



{% endhighlight %}



## Methods

### addItem()
{:#methods:additem} 

To add item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Add item at index 2" data-ej-touchend="add" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function add() {
            $("#listview").ejmListView("addItem", "New Item", 2);
        }
    </script>


{% endhighlight %}



### append()
{:#methods:append} 

To append new items with existing items.

#### Example

{% highlight html %}


    <script>
        window.listData = [{ name: "Charlotte Cooper" }, { name: "Shelley Burke" },
                    { name: "Regina Murphy" }, { name: "Yoshi Nagase" }, { name: "Antonio del Valle Saavedra" }]
        window.listNewData = [{ name: "Charlotte Cooper" }, { name: "Shelley Burke" },
                    { name: "Regina Murphy" }, { name: "Yoshi Nagase" }, { name: "Antonio del Valle Saavedra" },
                    { name: "Mayumi Ohno" }, { name: "Ian Devling" }]
    </script>

    <input data-role="ejmbutton" type="button" data-ej-text="Append" data-ej-touchend="append" />
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="name" data-ej-itemscount="3"></ul>

    <script>
        function append() {
            $("#listview").ejmListView("append", window.listNewData);
        }
    </script>


{% endhighlight %}



### checkAll()
{:#methods:checkall} 

To check all items in the ListView.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Check all items" data-ej-touchend="check" />
    <ul id="listview" data-role="ejmlistview" data-ej-enablechecklist="true">
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
    <script>
        function check() {
            $("#listview").ejmListView("checkAll");
        }
    </script>


{% endhighlight %}



### checkItemsByIndex()
{:#methods:checkitemsbyindex} 

To check item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Check item at index 2" data-ej-touchend="check" />
    <ul id="listview" data-role="ejmlistview" data-ej-enablechecklist="true" >
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
    <script>
        function check() {
            $("#listview").ejmListView("checkItemsByIndex", 2);
        }
    </script>


{% endhighlight %}



### checkItemsByIndices()
{:#methods:checkitemsbyindices} 

To check items in the given array of indices.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Check items at indices 2,3" data-ej-touchend="check" />
    <ul id="listview" data-role="ejmlistview" data-ej-enablechecklist="true">
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
    <script>
        function check() {
            $("#listview").ejmListView("checkItemsByIndices", [2,3]);
        }
    </script>


{% endhighlight %}



### deleteItemByIndex()
{:#methods:deleteitembyindex} 

To delete an item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Delete item at index 2" data-ej-touchend="deleteItem" />
    <ul id="listview" data-role="ejmlistview">
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
    <script>
        function deleteItem() {
            var index = $("#listview").ejmListView("deleteItemByIndex", 2);
            alert("Received index is: '" + index + "'");
        }
    </script>


{% endhighlight %}



### deleteItemByText()
{:#methods:deleteitembytext} 

To delete an item which having the text same as given string.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Delete item with text ‘Abstract’" data-ej-touchend="deleteItem" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function deleteItem() {
            $("#listview").ejmListView("deleteItemByText", "Abstract");
        }
    </script>


{% endhighlight %}



### deselectItem()
{:#methods:deselectitem} 

To deselect the item which is already selected.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Deselect item" data-ej-touchend="deselect" />
    <ul id="listview" data-role="ejmlistview" data-ej-selectedindex="2" data-ej-persistselection="true">
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
    <script>
        function deselect() {
            $("#listview").ejmListView("deselectItem");
        }
    </script>


{% endhighlight %}



### disable()
{:#methods:disable} 

To disable the ListView control.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable ListView" data-ej-touchend="disable" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function disable() {
            $("#listview").ejmListView("disable");
        }
    </script>


{% endhighlight %}



### disableAll()
{:#methods:disableall} 

To disable all items in the ListView.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable all items" data-ej-touchend="disable" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function disable() {
            $("#listview").ejmListView("disableAll");
        }
    </script>


{% endhighlight %}



### disableItemByIndex()
{:#methods:disableitembyindex} 

To disable item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable item at index 2" data-ej-touchend="disable" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function disable() {
            $("#listview").ejmListView("disableItemByIndex", 2);
        }
    </script>


{% endhighlight %}



### disableItemsByIndices()
{:#methods:disableitemsbyindices} 

To disable items in the given array of indices.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable items at indices 2,3" data-ej-touchend="disable" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function disable() {
            $("#listview").ejmListView("disableItemsByIndices", [2,3]);
        }
    </script>


{% endhighlight %}



### enable()
{:#methods:enable} 

To enable the ListView control.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Enable ListView" data-ej-touchend="enable" />
    <ul id="listview" data-role="ejmlistview" data-ej-enabled="false">
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
    <script>
        function enable() {
            $("#listview").ejmListView("enable");
        }
    </script>


{% endhighlight %}



### enableAll()
{:#methods:enableall} 

To enable all items in the ListView.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Enable all items" data-ej-touchend="enable" />
    <ul id="listview" data-role="ejmlistview">
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
    <script>
        $(function () {
            $("#listview").ejmListView("disableAll");
        });
        function enable() {
            $("#listview").ejmListView("enableAll");
        }
    </script>


{% endhighlight %}



### enableItemByIndex()
{:#methods:enableitembyindex} 

To enable item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Enable item at index 2" data-ej-touchend="enable" />
    <ul id="listview" data-role="ejmlistview" >
        <li data-ej-text="Artwork"></li>
        <li data-ej-text="Abstract"></li>
        <li data-ej-text="2 Acrylic Mediums" data-ej-enabled="false" ></li>
        <li data-ej-text="Creative Acrylic"></li>
        <li data-ej-text="Modern Painting"></li>
        <li data-ej-text="Canvas Art"></li>
        <li data-ej-text="Black white"></li>
        <li data-ej-text="Children"></li>
        <li data-ej-text="Preschool Crafts"></li>
        <li data-ej-text="School-age Crafts"></li>
    </ul>
    <script>
        function enable() {
            $("#listview").ejmListView("enableItemByIndex", 2);
        }
    </script>


{% endhighlight %}



### enableItemsByIndices()
{:#methods:enableitemsbyindices} 

To enable items in the given array of indices.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Enable items at indices 2,3" data-ej-touchend="enable" />
    <ul id="listview" data-role="ejmlistview" >
        <li data-ej-text="Artwork"></li>
        <li data-ej-text="Abstract"></li>
        <li data-ej-text="2 Acrylic Mediums" data-ej-enabled="false"></li>
        <li data-ej-text="Creative Acrylic" data-ej-enabled="false"></li>
        <li data-ej-text="Modern Painting"></li>
        <li data-ej-text="Canvas Art"></li>
        <li data-ej-text="Black white"></li>
        <li data-ej-text="Children"></li>
        <li data-ej-text="Preschool Crafts"></li>
        <li data-ej-text="School-age Crafts"></li>
    </ul>
    <script>
        function enable() {
            $("#listview").ejmListView("enableItemsByIndices", [2,3]);
        }
    </script>


{% endhighlight %}



### getIndexByText()
{:#methods:getindexbytext} 

To get the index of item which having same text as given string.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Get index of item with text ‘Abstract’" data-ej-touchend="get" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function get() {
            var index = $("#listview").ejmListView("getIndexByText", "Abstract");
            alert("Received index is: '" + index + "'");
        }
    </script>


{% endhighlight %}



### getItemByIndex()
{:#methods:getitembyindex} 

To get the item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Get item at index 2" data-ej-touchend="get" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function get() {
            var item = $("#listview").ejmListView("getItemByIndex", 2);
            alert("Received item is: '" + $(item).text() + "'");
        }
    </script>


{% endhighlight %}



### getItemByText()
{:#methods:getitembytext} 

To get the item which having same text as given string.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Get item with text ‘Abstract’" data-ej-touchend="get" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function get() {
            var item = $("#listview").ejmListView("getItemByText", "Abstract");
            alert("Received item is: '" + $(item).text() + "'");
        }
    </script>


{% endhighlight %}



### getTextByIndex()
{:#methods:gettextbyindex} 

To get the text of the item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Get 2nd item’s Text" data-ej-touchend="get" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function get() {
            var text = $("#listview").ejmListView("getTextByIndex", 2);
            alert("Received text is: '" + text + "'");
        }
    </script>


{% endhighlight %}



### selectItemByIndex()
{:#methods:selectitembyindex} 

To select item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Select item at index 2" data-ej-touchend="select" />
    <ul id="listview" data-role="ejmlistview" data-ej-persistselection="true" >
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
    <script>
        function select() {
            $("#listview").ejmListView("selectItemByIndex", 2);
        }
    </script>


{% endhighlight %}



### setBadge()
{:#methods:setbadge} 

To set badge value for an item.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Set badge value for item at index 2" data-ej-touchend="set" />
    <ul id="listview" data-role="ejmlistview" >
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
    <script>
        function set() {
            $("#listview").ejmListView("setBadge", 2, 33);
        }
    </script>


{% endhighlight %}



### uncheckAll()
{:#methods:uncheckall} 

To uncheck all items in the ListView.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Uncheck all items" data-ej-touchend="uncheck" />
    <ul id="listview" data-role="ejmlistview" data-ej-enablechecklist="true">
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
    <script>
        $(function () {
            $("#listview").ejmListView("checkAll");
        });
        function uncheck() {
            $("#listview").ejmListView("uncheckAll");
        }
    </script>


{% endhighlight %}



### uncheckItemsByIndex()
{:#methods:uncheckitemsbyindex} 

To uncheck item in the given index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Uncheck item at index 2" data-ej-touchend="uncheck" />
    <ul id="listview" data-role="ejmlistview" data-ej-enablechecklist="true">
        <li data-ej-text="Artwork"></li>
        <li data-ej-text="Abstract"></li>
        <li data-ej-text="2 Acrylic Mediums" data-ej-checkby="true"></li>
        <li data-ej-text="Creative Acrylic"></li>
        <li data-ej-text="Modern Painting"></li>
        <li data-ej-text="Canvas Art"></li>
        <li data-ej-text="Black white"></li>
        <li data-ej-text="Children"></li>
        <li data-ej-text="Preschool Crafts"></li>
        <li data-ej-text="School-age Crafts"></li>
    </ul>
    <script>
        function uncheck() {
            $("#listview").ejmListView("uncheckItemsByIndex", 2);
        }
    </script>


{% endhighlight %}



### uncheckItemsByIndices()
{:#methods:uncheckitemsbyindices} 

To uncheck items in the given array of indices.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Uncheck items at indices 2,3" data-ej-touchend="uncheck" />
    <ul id="listview" data-role="ejmlistview" data-ej-enablechecklist="true">
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
    <script>
        $(function () {
            $("#listview").ejmListView("checkItemsByIndices", [2,3]);
        });
        function uncheck() {
            $("#listview").ejmListView("uncheckItemsByIndices", [2, 3]);
        }
    </script>


{% endhighlight %}



## Events

### actionComplete
{:#events:actioncomplete} 

Event triggers after the AJAX content loaded completely.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
    </script>

    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="ContactName" data-ej-itemscount="5" data-ej-actioncomplete="complete"></ul>

    <script>
        function complete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### actionFailure
{:#events:actionfailure} 

Event triggers when the AJAX request failed.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
errorThrown</td><td>
Object</td><td>
Returns the error thrown in the AJAX post.</td></tr>
<tr>
<td>
textStatus</td><td>
Object</td><td>
Returns the status.</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current ListView item.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Returns the current item index.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}



    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/North.svc/Suppliers"
        });
    </script>

    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="ContactName" data-ej-itemscount="5" data-ej-actionfailure="failure"></ul>

    <script>
        function failure(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### actionSuccess
{:#events:actionsuccess} 

Event triggers after the AJAX content loaded successfully.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
    </script>

    <input data-role="ejmbutton" type="button" data-ej-text="Append" data-ej-touchend="append" />
    <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="ContactName" data-ej-itemscount="5" data-ej-actionsuccess="success"></ul>

    <script>
        function append() {
            $("#listview").ejmListView("append", window.listData);
        }
        function success(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### afterDelete
{:#events:afterdelete} 

Event triggers after an item deleted in ListView.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current ListView item.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Returns the current item index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the current item is checked or not.</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
Returns the current item is intractable or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Returns the current item is selected or not.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-deletemode="swipe" data-ej-afterdelete="afterdelete">
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

    <script>
        function afterdelete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ deleteMode: "swipe", afterDelete: "afterdelete" });
        function afterdelete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### beforeDelete
{:#events:beforedelete} 

Event triggers before an item deleted in ListView.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current ListView item.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Returns the current item index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the current item is checked or not.</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
Returns the current item is intractable or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Returns the current item is selected or not.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-deletemode="swipe" data-ej-beforedelete="beforedelete">
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

    <script>
        function beforedelete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ deleteMode: "swipe", beforeDelete: "beforedelete" });
        function beforedelete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}


### select
{:#events:select} 

Event triggers after an item selected in ListView.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the curent ListView item.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Returns the current item index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the current item is checked or not.</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
Returns the current item is intractable or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Returns the current item is selected or not.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-select="select">
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

    <script>
        function select(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ select: "select" });
        function select(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### touchEnd
{:#events:touchend} 

Event triggers when touch end happens on the item.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current ListView item.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Returns the current item index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the current item is checked or not.</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
Returns the current item is intractable or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Returns the current item is selected or not.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-touchend="touchend">
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

    <script>
        function touchend(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ touchEnd: "touchend" });
        function touchend(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### touchStart
{:#events:touchstart} 

Event triggers when touch start happens on the item.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from ListView.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current ListView item.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Returns the current item index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the current item is checked or not.</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
Returns the current item is intractable or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Returns the current item is selected or not.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="listview" data-role="ejmlistview" data-ej-touchstart="touchstart">
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

    <script>
        function touchstart(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="listview">
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

    <script>
        $("#listview").ejmListView({ touchStart: "touchstart" });
        function touchstart(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



