---
layout: post
title: ejmTab | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmTab
platform: Mobilejs
control: ejmTab
documentation: API
keywords: ejmTab, API, Essential Studio JS Tab (Mobile)
---

# ejmTab

The Essential JavaScript Mobile Tab widget is an interface where lists of tab contents switched between them while selection occurred on a tab item. Tabs are loaded through AJAX content.

Custom Design for HTML Tab control.

$(element).ejmTab()

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container" });
        });
    </script>



{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

## Members

### ajaxSettings
{:#members:ajaxSettings} 

Specifies for AJAX functionalities while loading contents through AJAX requests.

N> Set proper paths for [href] property to show contents properly

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-ajaxsettings-type="GET" data-ej-ajaxsettings-cache="false" data-ej-ajaxsettings-async="true" data-ej-ajaxsettings-datatype="html" data-ej-ajaxsettings-contenttype="html">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ 
                contentId: "tabdefault-container",
                enableAjax: true,
                ajaxSettings: {
                    type: 'GET',
                    cache: false,
                    async: true,
                    dataType: "html",
                    contentType: "html",
                    url: "",
                    data: {}
                }
            });
        });
    </script>



{% endhighlight %}

Text1.html:

{% highlight html %}


    <div id="default1">
        Movies content here
    </div>



{% endhighlight %}

Text2.html:

{% highlight html %}


    <div id="default2">
        Music content here
    </div>



{% endhighlight %}

Text3.html:

{% highlight html %}


    <div id="default2">
        Favourites content here
    </div>



{% endhighlight %}

### ajaxSettings.async `boolean`
{:#members:ajaxsettings-async}

It specifies, whether to enable or disable asynchronous request.


#### Default Value

* true


### ajaxSettings.cache `boolean`
{:#members:ajaxsettings-cache}

It specifies the page will be cached in the web browser.


#### Default Value

* false


### ajaxSettings.contentType `string`
{:#members:ajaxsettings-contenttype}

It specifies the type of data is send in the query string.



#### Default Value

* "html"



### ajaxSettings.data `object`
{:#members:ajaxsettings-data}


It specifies the data as an object, will be passed in the query string.


#### Default Value

* {}


### ajaxSettings.dataType `string`
{:#members:ajaxsettings-datatype}


It specifies the type of data that you're expecting back from the response.

#### Default Value

* "html"


### ajaxSettings.type `string`
{:#members:ajaxsettings-type}

It specifies the HTTP request type.


#### Default Value


* "get"

### ajaxSettings.url `string`
{:#members:ajaxsettings-url}

Specifies the URL to which the request is sent.


#### Default Value


* ""

### allowSwiping `boolean`
{:#members:allowSwiping} 

Specifies whether to enable swiping feature or not. This helps you to change tab by swiping the contents.

#### Default value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-allowswiping="false">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", allowSwiping: false });
        });
    </script>



{% endhighlight %}



### badge
{:#members:badge} 

Section for badge specific functionalities.

### badge.maxValue `number`
{:#members:badgemaxValue} 

Specifies the maximum value allowed for a badge.

#### Default value

* 100

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-badge-maxvalue="88">
        <li data-ej-href="#default1" data-ej-badge-value='90' data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-badge-value='73' data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-badge-value='90' data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-badge-value='73' data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", badge: { maxValue: 88 } });
        });
    </script>



{% endhighlight %}



### contentId `string`
{:#members:contentId} 

Specifies the id of the tab content container. Selected tab item’s contents will be visible inside this element.

#### Default value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container" });
        });
    </script>



{% endhighlight %}



### cssClass `string`
{:#members:cssClass} 

Sets the root class for Tab theme. This cssClass API helps to use custom skinning option for Tab control. By defining the root class using this API, we need to include this root class in CSS.

#### Default value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-cssclass="customclass">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <style>
        .customclass .e-m-tab-item {
            color: red !important;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", cssClass: "customclass" });
        });
    </script>

    <style>
        .customclass .e-m-tab-item {
            color: red !important;
        }
    </style>



{% endhighlight %}



### enableAjax `boolean`
{:#members:enableAjax} 

Specifies whether AJAX content will be used to load the tab contents.

#### Default value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true });
        });
    </script>



{% endhighlight %}

Text1.html:

{% highlight html %}


    <div id="default1">
        Movies content here
    </div>



{% endhighlight %}

Text2.html:

{% highlight html %}


    <div id="default2">
        Music content here
    </div>



{% endhighlight %}

Text3.html:

{% highlight html %}


    <div id="default2">
        Favourites content here
    </div>



{% endhighlight %}



### enableCache `boolean`
{:#members:enableCache} 

Specifies whether to enable Caching or not. If you are not enabling cache, each tab item change loads the contents after AJAX request. Otherwise tab contents loaded form browser cache.

N> Enable cache behavior works only for AJAX contents. This property is a dependent property of [enableAjax]. So [enabeAjax] must to be set as true.

#### Default value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-enablecache="true">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>



{% endhighlight %}



{% highlight html %}


  <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>    
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, enableCache: true });
        });
    </script>



{% endhighlight %}

Text1.html:

{% highlight html %}


    <div id="default1">
        Movies content here
    </div>



{% endhighlight %}

Text2.html:

{% highlight html %}


    <div id="default2">
        Music content here
    </div>



{% endhighlight %}

Text3.html:

{% highlight html %}


    <div id="default2">
        Favourites content here
    </div>



{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablePersistence} 

Saves current model value to browser cookies for state maintains. While refreshing the page retains the model value applies from browser cookies.

#### Default value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enablepersistence="true" >
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enablePersistence: true });
        });
    </script>



{% endhighlight %}



### enableRippleEffect `boolean`
{:#members:enableRippleEffect} 

Specifies whether to enable or disable ripple effect.

#### Default value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enablerippleeffect="true" >
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableRippleEffect: true });
        });
    </script>



{% endhighlight %}



### items `jsonarry`
{:#members:items} 

Specifies the tab items as an array of JSONobjects.

#### Default value

* []

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <script>
        window.items = [{ href: '#default1', text: 'Movies', icon: 'film' }, { href: '#default2', text: 'Music', icon: 'musicicon'  }, { href: '#default3', text: 'Favourites', icon: 'favourite' }]
    </script>

    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-items="window.items"></ul>
    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        </ul>
        <div id="tabdefault-container">
        </div>

        <div id="default1">
            Movies content here
        </div>
        <div id="default2">
            Music content here
        </div>
        <div id="default3">
            Favourites content here
        </div>

        <script>
            $(function () {
                $("#tab").ejmTab({ contentId: "tabdefault-container", items: [{ href: '#default1', text: 'Movies', icon: 'film' }, { href: '#default2', text: 'Music', icon: 'musicicon'  }, { href: '#default3', text: 'Favourites', icon: 'favourite' }] });
            });
        </script>


{% endhighlight %}


### itemStyle `enum`
{:#members:itemStyle} 

Specifies how the tab items will be visible in the screen. See [TabItemStyle](http://help.syncfusion.com/mobilejs/api/global#tabitemstyle)

#### Default value

* “bothblock”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-itemstyle="image">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", itemStyle: "image" });
        });
    </script>



{% endhighlight %}



### position `enum`
{:#members:position} 

Specifies the position of tab bar. i.e. top or bottom. 

#### Default value

* “bottom”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-position="top">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", position: "top" });
        });
    </script>



{% endhighlight %}



### prefetchAjaxContent `boolean`
{:#members:prefetchAjaxContent} 

Specifies whether need to pre fetch the AJAX content or not. If this set as true, all tab contents will be loaded initially. No further AJAX request will be initiated.

#### Default value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-prefetchajaxcontent="true">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, prefetchAjaxContent: true });
        });
    </script>



{% endhighlight %}

Text1.html:

{% highlight html %}


    <div id="default1">
        Movies content here
    </div>



{% endhighlight %}

Text2.html:

{% highlight html %}


    <div id="default2">
        Music content here
    </div>



{% endhighlight %}

Text3.html:

{% highlight html %}


    <div id="default2">
        Favourites content here
    </div>



{% endhighlight %}



### renderMode `enum`
{:#members:renderMode} 

Changes the rendering mode. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default value

* auto

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-rendermode="android">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", renderMode: "android"  });
        });
    </script>



{% endhighlight %}



### selectedItemIndex `number`
{:#members:selectedItemIndex} 

Specifies which item will be selected initially.

#### Default value

* 0

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-selecteditemindex="1">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", selectedItemIndex: 1 });
        });
    </script>



{% endhighlight %}



### showAjaxPopup `boolean`
{:#members:showAjaxPopup} 

Specifies whether show waiting popup in AJAX content loading or not.

#### Default value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-showajaxpopup="true">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text3.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, showAjaxPopup: true });
        });
    </script>



{% endhighlight %}

Text1.html:

{% highlight html %}


    <div id="default1">
        Movies content here
    </div>



{% endhighlight %}

Text2.html:

{% highlight html %}


    <div id="default2">
        Music content here
    </div>



{% endhighlight %}

Text3.html:

{% highlight html %}


    <div id="default2">
        Favourites content here
    </div>



{% endhighlight %}



## Methods

### addItem()
{:#methods:addItem} 

To add a tab item 

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Add item at index 2" data-ej-touchend="add" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>
    <div id="default4">
        Playlist content here
    </div>

    <script>
        function add() {
            $("#tab").ejmTab("addItem", "<li data-ej-text='Playlist' data-ej-icon='playmusic' data-ej-href='#default4'></li>", 2);
        }
    </script>



{% endhighlight %}

### disableContent()
{:#methods:disableContent} 

To disable any tab item content by its index

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Disable content of item at index 2" data-ej-touchend="disable" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function disable() {
            $("#tab").ejmTab("disableContent", 2);
        }
    </script>



{% endhighlight %}



### disableItem()
{:#methods:disableItem} 

To disable any tab item by its index

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Disable item at index 2" data-ej-touchend="disable" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function disable() {
            $("#tab").ejmTab("disableItem", 2);
        }
    </script>



{% endhighlight %}



### enableContent()
{:#methods:enableContent} 

To enable any tab item content which is already disabled by disableContent()

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Disable content of item at index 2" data-ej-touchend="disable" />
        <input data-role="ejmbutton" type="button" data-ej-text="Enable content of item at index 2" data-ej-touchend="enable" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function disable() {
            $("#tab").ejmTab("disableContent", 2);
        }
        function enable() {
            $("#tab").ejmTab("enableContent", 2);
        }
    </script>



{% endhighlight %}



### enableItem()
{:#methods:enableItem} 

To enable the tab item which is already disabled by disableItem()

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Disable item at index 2" data-ej-touchend="disable" />
        <input data-role="ejmbutton" type="button" data-ej-text="Enable item at index 2" data-ej-touchend="enable" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function disable() {
            $("#tab").ejmTab("disableItem", 2);
        }
        function enable() {
            $("#tab").ejmTab("enableItem", 2);
        }
    </script>



{% endhighlight %}



### getActiveItem()
{:#methods:getActiveItem} 

Get the current active item as html element

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Get active item" data-ej-touchend="get" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function get() {
            var item = $("#tab").ejmTab("getActiveItem");
            alert("Active item's id is: " + item[0].id);
        }
    </script>



{% endhighlight %}



### getActiveItemText()
{:#methods:getActiveItemText} 

Get the current active item’s text

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Get active item text" data-ej-touchend="get" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function get() {
            var itemtext = $("#tab").ejmTab("getActiveItemText");
            alert("Active item's text is: " + itemtext);
        }
    </script>



{% endhighlight %}



### getItemsCount()
{:#methods:getItemsCount} 

To return the tab item count

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Get items count" data-ej-touchend="get" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function get() {
            var itemtext = $("#tab").ejmTab("getItemsCount");
            alert("Total items exists: " + itemtext);            
        }
    </script>



{% endhighlight %}



### hideBadge()
{:#methods:hideBadge} 

To hide a badge

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-badge-value='90' data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-badge-value='73' data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Hide badge of item at index 1" data-ej-touchend="hide" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function hide() {
            $("#tab").ejmTab("hideBadge", 1);
        }
    </script>



{% endhighlight %}



### removeItem()
{:#methods:removeItem} 

To remove a tab item by its index

##### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Remove item at index 2" data-ej-touchend="remove" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function remove() {
            $("#tab").ejmTab("removeItem", 2);
        }
    </script>



{% endhighlight %}



### setActiveItem()
{:#methods:setActiveItem} 

To make the tab item to be active

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Set item at index 2 as active" data-ej-touchend="set" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function set() {
            $("#tab").ejmTab("setActiveItem", 2);
        }
    </script>



{% endhighlight %}



### setBadgeValue()
{:#methods:setBadgeValue} 

To update or set badge value for an item

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-badge-value='90' data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-badge-value='73' data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Update badgevalue to 32 for item at index 1" data-ej-touchend="set" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function set() {
            $("#tab").ejmTab("setBadgeValue", 1, 32);
        }
    </script>



{% endhighlight %}



### setContent()
{:#methods:setContent} 

to set the content for any tab item

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Set content for item at index 2" data-ej-touchend="set" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function set() {
            var item = $("#tab").ejmTab("setContent", "#default3");
        }
    </script>



{% endhighlight %}



### showBadge()
{:#methods:showBadge} 

To show the tab item’s badge.

#### Example

{% highlight html %}


    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container">
        <li data-ej-href="#default1" data-ej-badge-value='90' data-ej-icon="film" data-ej-text='Movies'>
        </li>
        <li data-ej-href="#default2" data-ej-badge-value='73' data-ej-icon="musicicon" data-ej-text='Music'>
        </li>
        <li data-ej-href="#default3" data-ej-icon="favourite" data-ej-text='Favourites'>
        </li>
    </ul>

    <div id="tabdefault-container">
        <input data-role="ejmbutton" type="button" data-ej-text="Hide badge of item at index 1" data-ej-touchend="hide" />
        <input data-role="ejmbutton" type="button" data-ej-text="Show badge of item at index 1" data-ej-touchend="show" />
    </div>

    <div id="default1">
        Movies content here
    </div>
    <div id="default2">
        Music content here
    </div>
    <div id="default3">
        Favourites content here
    </div>

    <script>
        function hide() {
            $("#tab").ejmTab("hideBadge", 1);
        }
        function show() {
            $("#tab").ejmTab("showBadge", 1);
        }
    </script>



{% endhighlight %}



## Events


### ajaxBeforeLoad
{:#events:ajaxBeforeLoad} 


Event triggers before the AJAX contents load.

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
Event parameters from tab<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
string</td><td>
Returns the tab model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
index</td><td>
int</td><td>
Returns the current selected item index</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the selected tab item’s text</td></tr>
<tr>
<td>
url</td><td>
string</td><td>
Returns the active item URL</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current active item</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-ajaxbeforeload="load">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function load(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, ajaxBeforeLoad: "load" });
        });
        function load(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### ajaxComplete
{:#events:ajaxComplete} 


Triggers when the AJAX requests complete. The request may get failed or succeed.

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
Event parameters from tab<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
string</td><td>
Returns the tab model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
index</td><td>
int</td><td>
Returns the current selected item index</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the selected tab item’s text</td></tr>
<tr>
<td>
url</td><td>
string</td><td>
Returns the active item URL</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current active item</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-ajaxcomplete="complete">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function complete(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, ajaxComplete: "complete" });
        });
        function complete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### ajaxError
{:#events:ajaxError} 


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
Event parameters from tab<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
string</td><td>
Returns the tab model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
index</td><td>
int</td><td>
Returns the current selected item index</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the tab item’s text</td></tr>
<tr>
<td>
url</td><td>
string</td><td>
Returns the active item URL</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current active item</td></tr>
<tr>
<td>
textStatus</td><td>
string</td><td>
Returns the status of the AJAX loading.(like error)</td></tr>
<tr>
<td>
errorThrown</td><td>
string</td><td>
return the type of error when loading the AJAX</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-ajaxerror="error">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function error(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, ajaxError: "error" });
        });
        function error(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### ajaxSuccess
{:#events:ajaxSuccess} 


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
Event parameters from tab<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
string</td><td>
Returns the tab model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
index</td><td>
int</td><td>
Returns the current selected item index</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the selected tab item’s text</td></tr>
<tr>
<td>
url</td><td>
string</td><td>
Returns the active item URL</td></tr>
<tr>
<td>
item</td><td>
object</td><td>
Returns the current active item</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-ajaxsuccess="success">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function success(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, ajaxSuccess: "success" });
        });
        function success(args) {
            //handle the event
        }
    </script>



{% endhighlight %}




### load
{:#events:load} 

Event triggers when the load happens in the Tab

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
Returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
Returns the Tab model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
Returns the name of the event</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-load="load">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function load(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, load: "load" });
        });
        function load(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### loadComplete
{:#events:loadComplete} 

Event triggers when the loadComplete happens in the Tab

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
Returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
Returns the Tab model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
Returns the name of the event</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-loadcomplete="loadcomplete">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function loadcomplete(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, loadComplete: "loadcomplete" });
        });
        function loadcomplete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### select
{:#events:select} 

Event triggers when a tab item selected

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
Returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
Returns the Tab model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
argument.item</td><td>
object</td><td>
Returns the selected Tab element</td></tr>
<tr>
<td>
argument.index</td><td>
int</td><td>
Returns the current selected item index</td></tr>
<tr>
<td>
argument.text</td><td>
string</td><td>
Returns the selected tab item’s text</td></tr>
<tr>
<td>
argument.id</td><td>
string</td><td>
Returns the name of the id</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-select="select">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function select(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, select: "select" });
        });
        function select(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### touchEnd
{:#events:touchEnd} 

Event triggers when the touchEnd happens in the Tab

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
Returns the Tab model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
argument.item</td><td>
object</td><td>
Returns the selected Tab element</td></tr>
<tr>
<td>
argument.index</td><td>
int</td><td>
Returns the current selected item index</td></tr>
<tr>
<td>
argument.text</td><td>
string</td><td>
Returns the selected tab item’s text</td></tr>
<tr>
<td>
argument.id</td><td>
string</td><td>
Returns the name of the id</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-touchend="touchend">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function touchend(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, touchEnd: "touchend" });
        });
        function touchend(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### touchStart
{:#events:touchStart} 

Event triggers when the touchStart happens in the Tab

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
Returns the Tab model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
argument.item</td><td>
object</td><td>
Returns the selected Tab element</td></tr>
<tr>
<td>
argument.index</td><td>
int</td><td>
Returns the current selected item index</td></tr>
<tr>
<td>
argument.text</td><td>
string</td><td>
Returns the selected tab item’s text</td></tr>
<tr>
<td>
argument.id</td><td>
string</td><td>
Returns the name of the id</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <ul id="tab" data-role="ejmtab" data-ej-contentid="tabdefault-container" data-ej-enableajax="true" data-ej-touchstart="touchstart">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

<script>
    function touchstart(args) {
        //handle the event
    }
</script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <ul id="tab">
        <li data-ej-text="Movies" data-ej-icon="film" data-ej-href="text1.html"></li>
        <li data-ej-text="Music" data-ej-icon="musicicon" data-ej-href="text2.html"></li>
        <li data-ej-text="Favourites" data-ej-icon="favourite" data-ej-href="text4.html"></li>
    </ul>

    <div id="tabdefault-container">
    </div>

    <script>
        $(function () {
            $("#tab").ejmTab({ contentId: "tabdefault-container", enableAjax: true, touchStart: "touchstart" });
        });
        function touchstart(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



