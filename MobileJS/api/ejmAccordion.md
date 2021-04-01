---
layout: post
title: ejmAccordion | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmAccordion
platform: Mobilejs
control: ejmAccordion
documentation: API
keywords: ejmAccordion, API, Essential Studio JS Accordion (Mobile) 
---


# ejmAccordion


The Essential JavaScript Mobile Accordion widget is an interface where lists of items are collapsed or expanded. 

Custom Design for HTML Accordion control.

$(element).ejmAccordion()


#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="accordion" data-role="ejmaccordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion();
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

### ajaxSettings `Object`
{:#members:ajaxsettings}

Specifies the 'ajaxSettings' option to load the content to the accordion control.

#### Default Value

* null

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
  <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true"
        data-ej-ajaxsettings-type="GET" data-ej-ajaxsettings-cache="false" data-ej-ajaxsettings-async="true" data-ej-ajaxsettings-datatype="html" data-ej-ajaxsettings-contenttype="html">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({
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

### ajaxSettings.async `Boolean`
{:#members:ajaxsettings-async}

It specifies, whether to enable or disable asynchronous request.

### ajaxSettings.cache `Boolean`
{:#members:ajaxsettings-cache}

It specifies the page will be cached in the web browser.

### ajaxSettings.contentType `String`
{:#members:ajaxsettings-contenttype}

It specifies the type of data is send in the query string.

### ajaxSettings.data `Object`
{:#members:ajaxsettings-data}

It specifies the data as an object, will be passed in the query string.

### ajaxSettings.dataType `String`
{:#members:ajaxsettings-datatype}

It specifies the type of data that you're expecting back from the response.

### ajaxSettings.type `String`
{:#members:ajaxsettings-type}

It specifies the HTTP request type.

### collapseAll `Boolean`
{:#members:collapseall}

Specifies whether the panels to be collapsible.

#### Default Value:

* false

#### Example

{% highlight html %}

   <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-collapseall="true">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisiticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ collapseAll: true });
        });
    </script>


{% endhighlight %}



### cssClass `String`
{:#members:cssclass}

Sets the root class for Accordion theme. This cssClass API helps to use custom skinning option for Accordion control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* “”

#### Example

{% highlight html %}

   <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-cssclass="customclass">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ cssClass: "customclass" });
        });
    </script>


{% endhighlight %}

### disabledItems `Array`
{:#members:disableditems}

Specifies the indices of the item to be disabled.

#### Default Value:

* []

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-disableditems="[1]">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ disabledItems: [1] });
        });
    </script>


{% endhighlight %}



### enableAjax `Boolean`
{:#members:enableajax}

Specifies whether to load the Ajax content while selecting the panel header. 

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>

    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({ enableAjax: true });
        });
    </script>


{% endhighlight %}



### enableCache `Boolean`
{:#members:enablecache}

Specifies whether to enable caching the content.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-enablecache="true">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>

    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({ enableAjax: true, enableCache: true });
        });
    </script>


{% endhighlight %}



### enableMultipleOpen `Boolean`
{:#members:enablemultipleopen}

Specifies whether to activate multiple content panels at a time.

#### Default Value:

* false

#### Example

{% highlight html %}

   <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-enablemultipleopen="true">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ enableMultipleOpen: true });
        });
    </script>


{% endhighlight %}



### enablePersistence `Boolean`
{:#members:enablepersistence}

Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.

#### Default Value:

* false

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-enablepersistence="true">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ enablePersistence: true });
        });
    </script>


{% endhighlight %}



### enableRippleEffect `Boolean`
{:#members:enablerippleeffect}

Specifies the ripple effect for the Accordion control. By default in android mode its value is true and other render mode we need to set as true.

#### Default Value:

* ej.isAndroid()?true:false

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-enablerippleeffect="true">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ enableRippleEffect: true });
        });
    </script>


{% endhighlight %}



### expandAll `Boolean`
{:#members:expandall}

To expand all the panel item.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-expandall="true">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ expandAll: true });
        });
    </script>


{% endhighlight %}


### headerIcon
{:#members:headericon}

Specifies the accordion header icon.

### headerIcon.active `String`
{:#members:headericon-active}

Specifies the accordion active mode header icon.

#### Default Value:

* “e-m-icon-up”

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-headericon-active="e-m-icon-up">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ headerIcon: { active: "e-m-icon-up" } });
        });
    </script>


{% endhighlight %}



### headerIcon.normal `String`
{:#members:headericon-normal}

Specifies the accordion normal mode header icon.

#### Default Value:

* “e-m-icon-down”

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-headericon-normal="e-m-icon-down">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>	
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ headerIcon: { normal: "e-m-icon-down" } });
        });
    </script>


{% endhighlight %}



### heightAdjustMode `Enum`
{:#members:heightadjustmode}

Specifies the height style of the control. See heightAdjustMode

#### Default Value:

* “content”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-heightadjustmode="fill">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>	
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ heightAdjustMode: "fill" });
        });
    </script>


{% endhighlight %}





### locale `String`
{:#members:locale}

Change the Accordion text format based on given culture.

Default Value

* “en-US”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-locale="zh-CN">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>

     <script>
            ej.mobile.Accordion.Locale["zh-CN"] = {
                spinnerText: "加载 "
            };
    </script>

{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>

    <script>
           $("#accordion_loadondemand").ejmAccordion({enableAjax: true,locale:"zh-CN"})
            ej.mobile.Accordion.Locale["zh-CN"] = {
                spinnerText: "加载 "
            };
</script>


{% endhighlight %}


### prefetchAjaxContent `Boolean`
{:#members:prefetchajaxcontent}

Specifies whether to fetch the Ajax content initially.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-prefetchajaxcontent="true">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({ enableAjax: true, prefetchAjaxContent: true });
        });
    </script>


{% endhighlight %}



### renderMode `Enum`
{:#members:rendermode}

Changes the rendering mode of the accordion. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value:

* auto

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-rendermode="auto">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ renderMode: "auto" });
        });
    </script>


{% endhighlight %}



### selectedItems `Array`
{:#members:selecteditems}

Specifies the indices of items that need to be in active state or initialization.

#### Default Value:

* [0]

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-selecteditems="[1]">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ selectedItems: [1] });
        });
    </script>


{% endhighlight %}



### showAjaxPopup `Boolean`
{:#members:showajaxpopup}

Specifies to show the waiting popup when loading the Ajax content.

#### Default Value:

* false

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-showajaxpopup="true">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({ enableAjax: true, showAjaxPopup: true });
        });
    </script>


{% endhighlight %}



### showHeaderIcon `Boolean`
{:#members:showheadericon}

Specifies to show or hide the accordion header icon.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-showheadericon="false">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>


{% endhighlight %}





{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ showHeaderIcon: false });
        });
    </script>


{% endhighlight %}





### spinnerText `String`
{:#members:spinnertext}

Specifies the 'spinnerText' while ajax content loading.

#### Default Value:

* “Loading…”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-spinnertext="Waiting..." data-ej-enableajax="true">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>

    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({ spinnerText: "Waiting...", enableAjax: true })
        });
    </script>


{% endhighlight %}



## Methods

### addItem()
{:#methods:additem}

To add the panel items.

#### Example

{% highlight html %}

   <ul id="sample">
        <li data-ej-href="text1.html">Model-view-controller</li>
        <li data-ej-href="text2.html">WPF</li>
        <li data-ej-href="text3.html">WCF</li>
    </ul>
    <script>
        $(function () {
            $("#sample").ejmAccordion({ enableAjax: true });
            $("#sample").ejmAccordion("addItem", "<li data-ej-href='text2.html'>Other</li>", 2);
        })
    </script>


{% endhighlight %}



### deselectItems()
{:#methods:deselectitems}

To deSelect the panel items.

#### Example

{% highlight html %}

    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({ enableMultipleOpen: true });
            $("#accordion").ejmAccordion("deselectItems", [0]);
        });
    </script>


{% endhighlight %}



### disableItems()
{:#methods:disableitems}

To disable the panel items.

#### Example

{% highlight html %}

    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion();
            $("#accordion").ejmAccordion("disableItems", [0]);
        });
    </script>


{% endhighlight %}



### enableItems()
{:#methods:enableitems}

To enable the panel items.

#### Example

{% highlight html %}

    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion();
            $("#accordion").ejmAccordion("enableItems", [0]);
        });
    </script>


{% endhighlight %}



### getItemsCount()
{:#methods:getitemscount}

To get the panel items count.

#### Example

{% highlight html %}

<div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion();
            $("#accordion").ejmAccordion("getItemsCount");
        });
    </script>


{% endhighlight %}



### removeItem()
{:#methods:removeitem}

To remove the panel item.

#### Example

{% highlight html %}

<ul id="sample">
        <li data-ej-href="text1.html">Model-view-controller</li>
        <li data-ej-href="text2.html">WPF</li>
        <li data-ej-href="text3.html">WCF</li>
    </ul>
    <script>
        $(function () {
            $("#sample").ejmAccordion({ enableAjax: true });
            $("#sample").ejmAccordion("removeItem", 1);
        })
    </script>


{% endhighlight %}



### selectItems()
{:#methods:selectitems}

To select the panel items.

#### Example

{% highlight html %}

    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion();
            $("#accordion").ejmAccordion("selectItems", [1]);
        });
    </script>


{% endhighlight %}



## Events

### ajaxBeforeLoad
{:#events:ajaxbeforeload}

Event triggers before the Ajax contents load.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
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
Returns the spinner text</td></tr>
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
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-ajaxbeforeload="beforeLoad">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        function beforeLoad(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        $(function (args) {
            $("#accordion_loadondemand").ejmAccordion({
                enableAjax: true,
                ajaxBeforeLoad: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### ajaxComplete
{:#events:ajaxcomplete}

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
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
Returns the spinner text</td></tr>
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
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-ajaxcomplete="ajaxComplete">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        function ajaxComplete(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({
                enableAjax: true,
                ajaxComplete: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### ajaxError
{:#events:ajaxerror}

Event triggers when the Ajax request failed.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
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
Returns the spinner text</td></tr>
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
Return the status of the ajax loading.(like error)</td></tr>
<tr>
<td>
errorThrown</td><td>
string</td><td>
Return the type of error when loading the Ajax Data. </td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-ajaxerror="ajaxError">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        function ajaxError(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({
                enableAjax: true,
                ajaxError: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### ajaxSuccess
{:#events:ajaxsuccess}

Event triggers after the Ajax content loaded successfully.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
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
Returns the spinner text</td></tr>
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
    <ul id="accordion_loadondemand" data-role="ejmaccordion" data-ej-enableajax="true" data-ej-ajaxsuccess="ajaxSuccess">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        function ajaxSuccess(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <ul id="accordion_loadondemand">
        <li data-ej-text="Model-View-Controller" data-ej-href="text1.html"></li>
        <li data-ej-text="WPF" data-ej-href="text2.html"></li>
        <li data-ej-text="WCF" data-ej-href="text3.html"></li>
    </ul>
    <script>
        $(function () {
            $("#accordion_loadondemand").ejmAccordion({
                enableAjax: true,
                ajaxSuccess: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### collapse
{:#events:collapse}

Event triggers when the accordion items gets collapsed.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
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
item</td><td>
object</td><td>
Returns the current active item</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-collapse="onCollapse">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        function onCollapse(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({
                collapse: function (args) {                    
                    //handle the event
                }
            })
        });
    </script>


{% endhighlight %}



### expand
{:#events:expand}

Event triggers when the accordion items is expand.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
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
item</td><td>
object</td><td>
Returns the current active item</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-expand="onExpand">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        function onExpand(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({
                expand: function (args) {                    
                    //handle the event
                }
            })
        });
    </script>


{% endhighlight %}



### itemTouchEnd
{:#events:itemtouchend}

Event triggers when the touch end happens in the accordion items.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
index</td><td>
string</td><td>
Returns the current selected item index</td></tr>
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
    <div id="accordion" data-role="ejmaccordion" data-ej-itemtouchend="touchEnd">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        function touchEnd(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({
                itemTouchEnd: function (args) {
                    //handle the event
                }
            })
        });
    </script>


{% endhighlight %}



### itemTouchStart
{:#events:itemtouchstart}

Event triggers when the touch start happens in the accordion items.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
index</td><td>
string</td><td>
Returns the current selected item index</td></tr>
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
    <div id="accordion" data-role="ejmaccordion" data-ej-itemtouchstart="touchStart">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        function touchStart(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({
                itemTouchStart: function (args) {
                    //handle the event
                }
            })
        });
    </script>


{% endhighlight %}



### select
{:#events:select}

Event triggers when we select the accordion items.

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
Event parameters from accordion<table><br><tr><br><th>
<b>Name</b></th><th>
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
Returns the accordion model</td></tr>
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
item</td><td>
object</td><td>
Returns the current active item</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="accordion" data-role="ejmaccordion" data-ej-select="onSelect">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        function onSelect(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="accordion">
        <ul>
            <li data-ej-text="Inbox">
                <div>
                    All WinRT controls are optimized for touch, supporting common gestures: zooming,
                    panning, selecting, double-tapping, rotating, resizing.
                </div>
            </li>
            <li data-ej-text="Sent">
                <div>
                    All the components in the ASP. NET MVC Essential Studio have been built from the
                    ground up with performance in mind and are extremely lightweight.
                </div>
            </li>
            <li data-ej-text="Trash">
                <div>
                    With our sophisticated Direct-Trac support system, built from the ground up to
                    support enterprise customers, you will have a streamlined experience working with
                    our support team.
                </div>
            </li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#accordion").ejmAccordion({
                select: function (args) {
                    //handle the event
                }
            })
        });
    </script>


{% endhighlight %}







