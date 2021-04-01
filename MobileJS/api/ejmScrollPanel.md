---
layout: post
title: ejmScrollPanel | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmScrollPanel
platform: Mobilejs
control: ejmScrollPanel
documentation: API
keywords: ejmScrollPanel, API, Essential Studio JS Scrollpanel (Mobile) 
---

#ejmScrollPanel


The Essential JavaScript Mobile ScrollPanel widget is an interactive panel for scrolling. The Scroll Panel control wraps its contents in a scrollable area as an object in a GUI where continuous text, pictures are scrolled and viewed though it does not fits into the space of a mobile or computer display.

Custom Design for HTML Scrollpanel control.

$(element).ejmScrollPanel()


#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
 <div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>


{% endhighlight %}



#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

* module:ej.mobile.scrollbar



## Members

### allowPullToRefresh `Boolean`
{:#members:allowpulltorefresh}

Specifies whether to enable the pull to refresh.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
    <div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-allowpulltorefresh="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                allowPullToRefresh: true
            });
        });
    </script>


{% endhighlight %}



### bounceTime `Int`
{:#members:bouncetime}

Specifies the bouncing time when bouncing behavior is enabled.

#### Default Value:

* 450

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-bouncetime=1000></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                bounceTime: 1000
            });
        });
    </script>


{% endhighlight %}



### cssClass `String`
{:#members:cssclass}

Sets the root class for scrollpanel. This cssClass API helps to use custom skinning option for scrollpanel control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* ””

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-cssclass="customclass"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                cssClass: "customclass"
            });
        });
    </script>


{% endhighlight %}


### deceleration `Int`
{:#members:deceleration}

Specifies the deceleration value.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-rendermode="windows" data-ej-deceleration="0.00006"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                renderMode: "windows",
                deceleration: 0.00006
            });
        });
    </script>


{% endhighlight %}



### directionLockThreshold `Int`
{:#members:directionlockthreshold}

Specifies the value for direction lock threshold.

#### Default Value:

* 5

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-directionlockthreshold=12></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                directionLockThreshold: 12
            });
        });
    </script>


{% endhighlight %}



### disableTouch `Boolean`
{:#members:disabletouch}

Specifies whether to disable touch.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-disabletouch="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                disableTouch: true
            });
        });
    </script>


{% endhighlight %}



### displacementTime `Int`
{:#members:displacementtime}

Specifies the displacement time.

#### Default Value:

* 800

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-displacementtime="1000" data-ej-enabledisplacement="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableDisplacement: true,
                displacementTime: 1000
            });
        });
    </script>


{% endhighlight %}



### displacementValue `Int`
{:#members:displacementvalue}

Specifies the displacement value.

#### Default Value:

* 94

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-displacementvalue="100" data-ej-enabledisplacement="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableDisplacement: true,
                displacementValue: 100
            });
        });
    </script>


{% endhighlight %}



### enableBounce `Boolean`
{:#members:enablebounce}

Specifies whether to enable bouncing behavior.

#### Default Value:

* true

N> For Android platform this property is false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablebounce="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableBounce: true
            });
        });
    </script>


{% endhighlight %}


### enabled `Boolean`
{:#members:enabled}

Specifies whether to enable or disable the control.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enabled="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enabled: true
            });
        });
    </script>


{% endhighlight %}



### enableFade `Boolean`
{:#members:enablefade}

Specifies whether need to fade the scrollbars.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablefade="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableFade: true
            });
        });
    </script>


{% endhighlight %}



### enableHrScroll `Boolean`
{:#members:enablehrscroll}

Specifies whether need to enable the horizontal scrolling.

#### Default Value:

* false

N> For windows tablet horizontal scrolling is true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablehrscroll=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableHrScroll: true
            });
        });
    </script>


{% endhighlight %}



### enableInteraction `Boolean`
{:#members:enableinteraction}

Specifies whether need to enable the interactive scrollbars.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enableinteraction="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({ target: "maincontent", enableInteraction: true });
        });
    </script>


{% endhighlight %}



### enableKeys `Boolean`
{:#members:enablekeys}

Specifies whether to enable keys.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablekeys=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableKeys: false
            });
        });
    </script>


{% endhighlight %}



### enableMouseWheel `Boolean`
{:#members:enablemousewheel}

Specifies whether to enable mouse wheel scrolling.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablemousewheel=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableMouseWheel: false
            });
        });
    </script>


{% endhighlight %}



### enableNativeScrolling `Boolean`
{:#members:enablenativescrolling}

Specifies whether to enable device’s native scroll behavior.

#### Default Value:

* false

N> For Windows tablet, this property is true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablenativescrolling="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableNativeScrolling: true
            });
        });
    </script>


{% endhighlight %}



### enableResize `Boolean`
{:#members:enableresize}

Specifies whether need to resize the scrollbar.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enableresize="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableResize: true
            });
        });
    </script>


{% endhighlight %}



### enableShrink `Boolean`
{:#members:enableshrink}

Specifies whether need to shrink the scrollbars.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enableshrink="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableShrink: "scale"
            });
        });
    </script>


{% endhighlight %}





### enableTransform `Boolean`
{:#members:enabletransform}

Specifies whether to enable transform style for the control.

#### Default Value:

* true

#### Example

{% highlight html %}

 <!-- Unobtrusive way of rendering --> 
 <div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enabletransform=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableTransform: false
            });
        });
    </script>


{% endhighlight %}



### enableTransition `Boolean`
{:#members:enabletransition}

Specifies whether to enable transition effect for the control.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enabletransition=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableTransition: false
            });
        });
    </script>


{% endhighlight %}



### enableVrScroll `Boolean`
{:#members:enablevrscroll}

Specifies whether need to enable the vertical scrolling.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablevrscroll="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableVrScroll: true
            });
        });
    </script>


{% endhighlight %}



### enableZoom `Boolean`
{:#members:enablezoom}

Specifies whether to enable zooming.

#### Default Value:

* false

#### Example


{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablezoom="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({ target: "maincontent", enableZoom: true });
        });
    </script>


{% endhighlight %}



### eventPassthrough `Boolean`
{:#members:eventpassthrough}

Specifies whether to set the event pass through.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-eventpassthrough="vertical"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                eventPassthrough: "vertical"
            });
        });
    </script>


{% endhighlight %}



### invertWheel `Boolean`
{:#members:invertwheel}

Specifies whether to enable invert wheel.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-invertwheel="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                invertWheel: true
            });
        });
    </script>


{% endhighlight %}



### isRelative `Boolean`
{:#members:isrelative}

Specifies whether to sets the scrollpanel to relative position.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-isrelative="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                isRelative: true
            });
        });
    </script>


{% endhighlight %}



### preventDefault `Boolean`
{:#members:preventdefault}

Specifies whether to prevent default events.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-preventdefault=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                preventDefault: false
            });
        });
    </script>


{% endhighlight %}



### pullToRefreshSettings `Object`
{:#members:pulltorefreshsettings}

Specifies the pull to refresh settings.

### pullToRefreshSettings.textOnPull `String`
{:#members:pulltorefreshsettings-textonpull}

Specifies the pull to refresh text on Pull.

#### Default Value:

* “Pull to Refresh…”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-pulltorefreshsettings-textonpull="Refresh..." data-ej-allowpulltorefresh="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                allowPullToRefresh: true,
                pullToRefreshSettings: {
                    textOnPull: "Refresh..."
                }
            });
        });
    </script>


{% endhighlight %}



### pullToRefreshSettings.textOnRefresh `String`
{:#members:pulltorefreshsettings-textonrefresh}

Specifies the pull to refresh text on refresh.

#### Default Value:

* “Refreshing…”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-pulltorefreshsettings-textonrefresh="Updating..." data-ej-allowpulltorefresh="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                allowPullToRefresh: true,
                pullToRefreshSettings: {
                    textOnRefresh: "Updating..."
                }
            });
        });
    </script>


{% endhighlight %}



### pullToRefreshSettings.textOnRelease `String`
{:#members:pulltorefreshsettings-textonrelease}

Specifies the pull to refresh text on release.

#### Default Value:

* “Release to Refresh…”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-pulltorefreshsettings-textonrelease="Refresh..." data-ej-allowpulltorefresh="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                allowPullToRefresh: true,
                pullToRefreshSettings: {
                    textOnRelease: "Refresh..."
                }
            });
        });
    </script>


{% endhighlight %}



### pullToRefreshSettings.thresholdDistance `Int`
{:#members:pulltorefreshsettings-thresholddistance}

Specifies the pull to refresh threshold distance.

#### Default Value:

* 75

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-pulltorefreshsettings-thresholddistance="25" data-ej-allowpulltorefresh="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                allowPullToRefresh: true,
                pullToRefreshSettings: {
                    thresholdDistance: 25
                }
            });
        });
    </script>


{% endhighlight %}



### renderMode `Enum`
{:#members:rendermode}

Specifies the rendering mode of the control. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value:

* auto

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-rendermode="auto"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                renderMode: ej.mobile.RenderMode.Auto
            });
        });
    </script>


{% endhighlight %}



### scrollEndThresholdDistance `Int`
{:#members:scrollendthresholddistance}

Specifies the value for scroll end threshold distance.

#### Default Value:

* 5

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-scrollendthresholddistance="5"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                scrollEndThresholdDistance: 5
            });
        });
    </script>


{% endhighlight %}



### scrollHeight `Int`
{:#members:scrollheight}

Specifies the scroll height of the content.

#### Default Value:

* “auto”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-scrollheight="300"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                scrollHeight: 300
            });
        });
    </script>


{% endhighlight %}



### scrollWidth `Int`
{:#members:scrollwidth}

Specifies the scroll width of the content.

#### Default Value:

* “auto”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-scrollwidth="200"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                scrollWidth: "200"
            });
        });
    </script>


{% endhighlight %}



### showScrollbars `Boolean`
{:#members:showscrollbars}

Specifies whether need to show the scroll bars.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-showscrollbars="true"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                showScrollbars: true
            });
        });
    </script>


{% endhighlight %}



### startX `Int`
{:#members:startx}

Specifies the x position on initialize.

#### Default Value:

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-startx=0></div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                startX: 0
            });
        });
    </script>


{% endhighlight %}



### startY `Int`
{:#members:starty}

Specifies the y position on initialize.

#### Default Value:

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-starty=30></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({ target: "maincontent", startY: 0 });
        });
    </script>


{% endhighlight %}



### startZoom `Int`
{:#members:startzoom}

Specifies the initial zooming value.

#### Default Value:

* 1

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablezoom="true" data-ej-startzoom=2></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                enableZoom: true,
                startZoom: 2
            });
        });
    </script>


{% endhighlight %}



### targetHeight `Int`
{:#members:targetheight}

Specifies the target element height.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-targetheight="300"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                targetHeight: 300
            });
        });
    </script>


{% endhighlight %}



### target `String`
{:#members:target}

Specifies the target element.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent"
            });
        });
    </script>


{% endhighlight %}



### targetWidth `Int`
{:#members:targetwidth}

Specifies the target element width.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-targetwidth="200"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                targetWidth: 200
            });
        });
    </script>


{% endhighlight %}



### wheelSpeed `Int`
{:#members:wheelspeed}

Specifies the wheel speed.

#### Default Value:

* 16

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-wheelspeed=20></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                wheelSpeed: 20
            });
        });
    </script>


{% endhighlight %}



### zoomMax `Int`
{:#members:zoommax}

Specifies the maximum zoom value.

#### Default Value:

* 6

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-zoom="true" data-ej-zoommax=6></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                zoom: true,
                zoomMax: 6
            });
        });
    </script>


{% endhighlight %}



### zoomMin `Int`
{:#members:zoommin}

Specifies the minimum zoom value.

#### Default Value:

* 1

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-zoom="true" data-ej-zoommin=2></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel({
                target: "maincontent",
                zoom: true,
                zoomMin: 2
            });
        });
    </script>


{% endhighlight %}



## Methods

### disable()
{:#methods:disable}

To disable the scrollpanel.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        // Disable the scroll panel
        $(function () {
            $("#scrollpanel").ejmScrollPanel('disable');
        });
    </script>


{% endhighlight %}



### enable()
{:#methods:enable}

To enable the scrollpanel.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        // Enable the scroll panel
        $(function () {
            $("#scrollpanel").ejmScrollPanel('enable');
        });
    </script>


{% endhighlight %}



### getComputedPosition()
{:#methods:getcomputedposition}

To get the computed position.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel('getComputedPosition');
        });
    </script>


{% endhighlight %}



### getScrollPosition()
{:#methods:getscrollposition}

To get the scroll position.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel('getScrollPosition');
        });
    </script>


{% endhighlight %}



### refresh()
{:#methods:refresh}

To refresh the scrollpanel.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        // Refresh the scroll panel
        $(function () {
            $("#scrollpanel").ejmScrollPanel('refresh');
        });
    </script>


{% endhighlight %}



### scrollBy()
{:#methods:scrollby}

To make the content scroll with time and easing given.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        $(function () {
            var scroll = $("#scrollpanel").data("ejmScrollPanel");
            $("#maincontent").click(function () {
                scroll.scrollBy(100, 1000, 5, 10);
            });
        });
    </script>


{% endhighlight %}



### scrollTo()
{:#methods:scrollto}

To make the content scroll to the position given.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        $(function () {
            var scroll = $("#scrollpanel").data("ejmScrollPanel");
            $("#maincontent").click(function () {
                scroll.scrollTo(10, 10);
            });
        });
    </script>


{% endhighlight %}



### stop()
{:#methods:stop}

To stop the scrolling.

#### Example

{% highlight html %}

  <div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        $(function () {
            $("#scrollpanel").ejmScrollPanel('stop');
        });
    </script>



{% endhighlight %}



### zoom()
{:#methods:zoom}

To zoom the scroll content.

#### Example

{% highlight html %}

<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent"></div>
    <script>
        // Refresh the scroll panel
        $(function () {
            var scroll = $("#scrollpanel").data("ejmScrollPanel");
            $("#maincontent").click(function () {
                scroll.zoom(10, 1, 1, 1);
            });
        });
    </script>


{% endhighlight %}



## Events

### pull
{:#events:pull}

Event triggers when pull is happened in the control.

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
Event parameters from scrollpanel.<table><br><tr><br><th>
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

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-allowpulltorefresh="true" data-ej-pull="pull"></div>
    <script>
        // pull event for scrollpanel
        function pull(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        // pull event for scrollpanel
        $("#scrollpanel").ejmScrollPanel({
            target: "maincontent",
            allowPullToRefresh: true,
            pull: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### scroll
{:#events:scroll}

Event triggers when scroll happens on the control.

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
Event parameters from scrollpanel.<table><br><tr><br><th>
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
x</td><td>
int</td><td>
Returns the x position.</td></tr>
<tr>
<td>
y</td><td>
int</td><td>
Returns the y position.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-scroll="scroll"></div>
    <script>
        // scroll event for scrollpanel
        function scroll(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        // scroll event for scrollpanel
        $("#scrollpanel").ejmScrollPanel({
            target: "maincontent",
            scroll: function (args) { //handle the event
            }
        });
    </script>	


{% endhighlight %}



### scrollEnd
{:#events:scrollend}

Event triggers when scroll end happens on the control.

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
Event parameters from scrollpanel.<table><br><tr><br><th>
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
x</td><td>
int</td><td>
Returns the x position.</td></tr>
<tr>
<td>
y</td><td>
int</td><td>
Returns the y position.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-scrollend="scrollEnd"></div>
    <script>
        // scrollEnd event for scrollpanel
        function scrollEnd(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        // scrollEnd event for scrollpanel
        $("#scrollpanel").ejmScrollPanel({
            target: "maincontent",
            scrollEnd: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### scrollStart
{:#events:scrollstart}

Event triggers when scroll start happens on the control.

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
Event parameters from scrollpanel.<table><br><tr><br><th>
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
x</td><td>
int</td><td>
Returns the x position.</td></tr>
<tr>
<td>
y</td><td>
int</td><td>
Returns the y position.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-scrollstart="scrollStart"></div>
    <script>
        // scrollStart event for scrollpanel
        function scrollStart(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        // scrollStart event for scrollpanel
        $("#scrollpanel").ejmScrollPanel({
            target: "maincontent",
            scrollStart: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### scrollStop
{:#events:scrollstop}

Event triggers when scroll stop happens on the control.

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
Event parameters from scrollpanel.<table><br><tr><br><th>
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
x</td><td>
int</td><td>
Returns the x position.</td></tr>
<tr>
<td>
y</td><td>
int</td><td>
Returns the y position.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-scrollstop="scrollStop"></div>
    <script>
        // scrollStop event for scrollpanel
        function scrollStop(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        // scrollStop event for scrollpanel
        $("#scrollpanel").ejmScrollPanel({
            target: "maincontent",
            scrollStop: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### zoomEnd
{:#events:zoomend}

Event triggers when zoom end happens on the control.

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
Event parameters from scrollpanel.<table><br><tr><br><th>
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
x</td><td>
int</td><td>
Returns the x position.</td></tr>
<tr>
<td>
y</td><td>
int</td><td>
Returns the y position.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablezoom="true" data-ej-zoomend="zoomEnd"></div>
    <script>
        // zoomEnd event for scrollpanel
        function zoomEnd(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        // zoomEnd event for scrollpanel
        $("#scrollpanel").ejmScrollPanel({
            target: "maincontent",
            zoomEnd: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### zoomStart
{:#events:zoomstart}

Event triggers when zoom start happens on the control.

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
Event parameters from scrollpanel.<table><br><tr><br><th>
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
x</td><td>
int</td><td>
Returns the x position.</td></tr>
<tr>
<td>
y</td><td>
int</td><td>
Returns the y position.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering --> 
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-zoomstart="zoomStart"></div>
    <script>
        // zoomStart event for scrollpanel
        function zoomStart(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="maincontent">
        <div>
            Scroll content here
        </div>
    </div>
    <div id="scrollpanel"></div>
    <script>
        // zoomStart event for scrollpanel
        $("#scrollpanel").ejmScrollPanel({
            target: "maincontent",
            zoomStart: function (args) { //handle the event
            }
        });
    </script>	


{% endhighlight %}



