---
layout: post
title: ejmSlider | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmSlider
platform: Mobilejs
control: ejmSlider
documentation: API
keywords: ejmSlider, API, Essential Studio JS Slider (Mobile) 
---

# ejmSlider

The Essential JavaScript Mobile Slider widget provides support to select a value from a particular range as well as a range of value. 

Custom Design for Html slider control:

$(element).ejmSlider()


#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="slider" data-role="ejmslider"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="slider"></div>
    <script>
        // Create slider
        $(function () {
            $("#slider").ejmSlider();
        });
    </script>


{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.mobile.application

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch



## Members

### animationSpeed `Int`
{:#members:animationspeed}

Specifies the animation speed when animation is enabled.

#### Default Value:

* 400

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-animationspeed=1000 data-ej-enableanimation=true></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ enableAnimation: true, animationSpeed: 1000 });
        });
    </script>


{% endhighlight %}



### enableAnimation `Boolean`
{:#members:enableanimation}

Specifies whether to enable the animation.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-enableanimation=true></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ enableAnimation: false });
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
    <div id="slider" data-role="ejmslider" data-ej-enabled=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ enabled: false });
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
    <div id="slider" data-role="ejmslider" data-ej-enablepersistence=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ enablePersistence: false });
        });
    </script>


{% endhighlight %}



### enableRange `Boolean`
{:#members:enablerange}

Specifies whether to enable the range slider.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-enablerange=true></div>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        // Set slider enableRange on initialization.
        //To set enableRange API value
        $(function () {
            $("#slider").ejmSlider({ enableRange: true });
        });
    </script>


{% endhighlight %}



### incrementStep `Int`
{:#members:incrementstep}

Specifies the step value for increment. 

#### Default Value:

* 1

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-incrementstep=1></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        // Set slider incrementStep on initialization.
        //To set incrementStep API value
        $(function () {
            $("#slider").ejmSlider({ incrementStep: 1 });
        });
    </script>


{% endhighlight %}



### ios7
{:#members:ios7}

Section for ios7 mode specific functionalities.

### ios7.thumbStyle `Enum`
{:#members:ios7-thumbstyle}

Specifies the thumb style in ios7 mode. See[ThumbStyle](http://help.syncfusion.com/mobilejs/api/global#members:thumbstyle)

#### Default Value:

* ej.mobile.Slider.ThumbStyle.Normal.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-rendermode="ios7" data-ej-ios7-thumbstyle="small"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ renderMode: "ios7", ios7: { thumbStyle: ej.mobile.Slider.ThumbStyle.Small } });
        });
    </script>


{% endhighlight %}



### maxValue `Int`
{:#members:maxvalue}

Specifies the maximum value.

#### Default Value:

* 100

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-maxvalue=100></div>


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ maxValue: 100 });
        });
    </script>


{% endhighlight %}



### minValue `Int`
{:#members:minvalue}

Specifies the minimum value.

#### Default Value:

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-minvalue=0></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ minValue: 0 });
        });
    </script>


{% endhighlight %}


### orientation `Enum`
{:#members:orientation}

Specifies whether the orientation is horizontal or vertical. See[Orientation](http://help.syncfusion.com/mobilejs/api/global#members:orientation)

#### Default Value:

* ej.mobile.Slider.Orientation.Horizontal.

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-orientation="vertical"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ orientation: ej.mobile.Slider.Orientation.Vertical });
        });
    </script>


{% endhighlight %}



### readOnly `Boolean`
{:#members:readonly}

Specifies whether the control is read only.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-readonly=true></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ readOnly: true });
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
    <div id="slider" data-role="ejmslider" data-ej-rendermode="auto"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>	
    <script>
        $(function () {
            $("#slider").ejmSlider({ renderMode: ej.mobile.RenderMode.Android });
        });
    </script>


{% endhighlight %}



### value `Int`
{:#members:value}

Specifies the current value.

#### Default Value:

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-value=30></div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ value: 50 });
        });
    </script>


{% endhighlight %}



### values `Int[]`
{:#members:values}

Specifies the values when range slider is enabled.

#### Default Value:

* [20,80]

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="slider" data-role="ejmslider" data-ej-enablerange=true data-ej-values=[20,80]></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="slider"></div>
    <script>
        $(function () {
            $("#slider").ejmSlider({ enableRange: true, values: [20, 80] });
        });
    </script>


{% endhighlight %}



## Methods

### getValue()
{:#methods:getvalue}

To get the current value.

#### Example

{% highlight html %}

<div id="slider"></div>
    <script>
        // get the slider's current value        
        $(function () {
            $("#slider").ejmSlider();
            $("#slider").ejmSlider("getValue");
        });
    </script>


{% endhighlight %}



## Events

### change
{:#events:change}

Event triggers when the value changed.

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
Event parameters from slider.<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
returns the model value of the control.</td></tr>
<tr>
<td>
value</td><td>
int</td><td>
returns the current value of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="slider" data-role="ejmslider" data-ej-change="onChange"></div>
    <script>
        // Change event for slider
        function onChange(args) { //handle the event            
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="slider"></div>
    <script>
        //change event for slider
        $(function () {
            $("#slider").ejmSlider({
                change: function (args) { //handle the event                    
                }
            });
        });
    </script>


{% endhighlight %}



### load
{:#events:load}

Event triggers before the control get loaded.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Descrip</b><b>tion</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from slider.<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
returns the model value of the control.</td></tr>
<tr>
<td>
value</td><td>
int</td><td>
returns the current value of the control.</td></tr>
<tr>
<td>
values</td><td>
int[]</td><td>
returns the current range values of the control when range slider feature is enabled.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="slider" data-role="ejmslider" data-ej-load="onLoad"></div>
    <script>
        // Load event for slider
        function onLoad(args) { //handle the event            
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="slider"></div>
    <script>
        //Load event for slider
        $(function () {
            $("#slider").ejmSlider({
                load: function (args) { //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### slide
{:#events:slide}

Event triggers when touch move happens on the control.

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
Event parameters from slider.<table><br><tr><br><th>
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
value</td><td>
int</td><td>
Returns the current value of the control.</td></tr>
<tr>
<td>
values</td><td>
int[]</td><td>
Returns the current range values of the control when range slider feature is enabled.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="slider" data-role="ejmslider" data-ej-slide="onslide"></div>
    <script>
        // slide event for slider
        function onslide(args) { //handle the event            
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="slider"></div>
    <script>
        //Slide event for slider
        $(function () {
            $("#slider").ejmSlider({
                slide: function (args) { //handle the event                    
                }
            });
        });
    </script>


{% endhighlight %}



### touchEnd
{:#events:touchend}

Event triggers when touch end happens on the control.

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
Event parameters from slider.<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be cancelled; otherwise, false.</td></tr>
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
value</td><td>
int</td><td>
Returns the current value of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="slider" data-role="ejmslider" data-ej-touchend="onStop"></div>
    <script>
        // touchEnd event for slider
        function onStop(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="slider"></div>
    <script>
        //touchEnd event for slider
        $(function () {
            $("#slider").ejmSlider({
                touchEnd: function (args) { //handle the event               
                }
            });
        });
    </script>


{% endhighlight %}



### touchStart
{:#events:touchstart}

Event triggers when touch start happens on the control.

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
Event parameters from slider.<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be cancelled; otherwise, false.</td></tr>
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
value</td><td>
int</td><td>
Returns the current value of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="slider" data-role="ejmslider" data-ej-touchstart="onStart"></div>
    <script>
        // touchStart event for slider
        function onStart(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="slider"></div>
    <script>
        //touchStart event for slider
        $(function () {
            $("#slider").ejmSlider({
                touchStart: function (args) { //handle the event                    
                }
            });
        });
    </script>


{% endhighlight %}




