---
layout: post
title: ejmRadialSlider | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmRadialSlider
platform: Mobilejs
control: ejmRadialSlider
documentation: API
keywords: ejmRadialSlider, API, Essential Studio JS RadialSlider (Mobile)
---

# ejmRadialSlider

Essential JavaScript Mobile RadialSlider control provides support to select a value from a particular range of values aligned in circular diagrammatic manner. The Range Slider has a needle to select the value and it is fixed with a base circle.

Custom Design for HTML RadialSlider control.

$(element).ejmRadialSlider()

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider"></div>

{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>
    
    <script>
        $("#defaultradialslider").ejmRadialSlider();
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

### autoOpen `boolean`
{:#members:autoopen} 

Specifies whether the radialslider control will be opened initially or not. 

N> If autoOpen property set as false, you need to handle radial slider open manually.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
        <br />
        <p>
            Click the button to open RadialSlider
        </p>
        <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialslideropen" data-ej-text="Open"></button>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-autoopen="false"></div>

    <script>
        function radialslideropen(args) {
            $("#defaultradialslider").ejmRadialSlider("show");
        }
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
        <br />
        <p>
            Click the button to open RadialSlider
        </p>
        <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialslideropen" data-ej-text="Open"></button>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ autoOpen: false });
        function radialslideropen(args) {
            $("#defaultradialslider").ejmRadialSlider("show");
        }
    </script>


{% endhighlight %}



### cssClass `string`
{:#members:cssclass} 

Sets the root class for RadialSlider theme. This cssClass API helps to use custom skinning option for RadialSlider control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-cssclass="customclass"></div>

    <style>
        .customclass .e-m-ticks-text {
            fill: red !important;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ cssClass: "customclass" });
    </script>

    <style>
        .customclass .e-m-ticks-text {
            fill: red !important;
        }
    </style>



{% endhighlight %}



### enableAnimation `boolean`
{:#members:enableanimation} 

To enable Animation for RadialSlider control.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
        <br />
        <p>
            Click the button to open RadialSlider
        </p>
        <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialslideropen" data-ej-text="Open"></button>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-autoopen="false" data-ej-enableanimation="false"></div>

    <script>
        function radialslideropen(args) {
            $("#defaultradialslider").ejmRadialSlider("show");
        }
    </script>


{% endhighlight %}



{% highlight html %}




    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
        <br />
        <p>
            Click the button to open RadialSlider
        </p>
        <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialslideropen" data-ej-text="Open"></button>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ autoOpen: false, enableAnimation: false });
        function radialslideropen(args) {
            $("#defaultradialslider").ejmRadialSlider("show");
        }
    </script>



{% endhighlight %}



### enableRoundOff `boolean`
{:#members:enableroundoff} 

Specifies the result value should be whole number or with decimals for the RadialSlider control.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-enableroundoff="false"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ enableRoundOff: false });
    </script>



{% endhighlight %}



### labelSpace `number`
{:#members:labelspace} 

Specifies the space between stroke and values in RadialSlider control.

#### Default Value

* 30

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-labelspace="50"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ labelSpace: 50 });
    </script>



{% endhighlight %}


### position `enum`
{:#members:position} 

Changes the Position of the control. See [RadialSliderPosition](http://help.syncfusion.com/mobilejs/api/global#radialsliderposition)

#### Default Value

* “rightcenter”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-position="bottomleft"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ position: "bottomleft" });
    </script>



{% endhighlight %}



### radius `number`
{:#members:radius} 

Specifies the radius of the RadialSlider control.

#### Default Value

* 200

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-radius="150"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ radius: 150 });
    </script>



{% endhighlight %}



### renderMode `enum`
{:#members:rendermode} 

Changes the rendering mode. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-rendermode="android"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ renderMode: "windows" });
    </script>



{% endhighlight %}



### strokeWidth `number`
{:#members:strokewidth} 

Specifies the radius of the RadialSlider control.

#### Default Value

* If windows or flat rendering mode, then the value is 12, otherwise 5

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-strokeWidth ="2"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({strokeWidth :2});
    </script>



{% endhighlight %}



### ticks `numberarray`
{:#members:ticks} 

Specifies the increment steps of RadialSlider control.

#### Default Value

* [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100]

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-ticks="[0, 25, 50, 75, 100]"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ ticks: [0, 25, 50, 75, 100] });
    </script>



{% endhighlight %}



### value `number`
{:#members:value} 

Specifies the value of the RadialSlider control need to be set initially.

#### Default Value

* 10

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-value="0"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider();
    </script>



{% endhighlight %}



## Methods

### hide()
{:#methods:hide} 

To hide the RadialSlider. You can’t access RadialSlider after this method called.

#### Example

{% highlight html %}


    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
        <br />
        <p>
            Click the button to hide RadialSlider
        </p>
        <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialsliderclose" data-ej-text="Hide"></button>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-autoopen="true"></div>

    <script>
        function radialsliderclose(args) {
            $("#defaultradialslider").ejmRadialSlider("hide");
        }
    </script>



{% endhighlight %}



### show()
{:#methods:show} 

To Show the RadialSlider

#### Example

{% highlight html %}


    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
        <br />
        <p>
            Click the button to show RadialSlider
        </p>
        <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialslideropen" data-ej-text="Show"></button>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-autoopen="false"></div>

    <script>
        function radialslideropen(args) {
            $("#defaultradialslider").ejmRadialSlider("show");
        }
    </script>



{% endhighlight %}



## Events

### change
{:#events:change} 

Event triggers while a value changed to new value in RadialSlider.

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
Event parameters from Radialslider<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the Radialslider model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
oldValue</td><td>
number</td><td>
Returns the previous value of RadialSlider</td></tr>
<tr>
<td>
value</td><td>
number</td><td>
Returns the currently selected value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-change="change"></div>

    <script>
        function change(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ change: "change" });
        function change(args) {
            //handle the event
        }
    </script> 



{% endhighlight %}



### slide
{:#events:slide} 

Event triggers while user slide the RadialSlider to change the value.

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
Event parameters from RadialSlider<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the RadialSlider model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
selectedValue</td><td>
number</td><td>
Returns the previous selected value of RadialSlider</td></tr>
<tr>
<td>
value</td><td>
number</td><td>
Returns the current value where the cursor in.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-slide="slide"></div>

    <script>
        function slide(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ slide: "slide" });
        function slide(args) {
            //handle the event
        }
    </script> 



{% endhighlight %}



### start
{:#events:start} 

Event triggers while user start sliding to change new value in RadialSlider.

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
Event parameters from RadialSlider<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the RadialSlider model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
number</td><td>
Returns the currently value before slide</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-start="start"></div>

    <script>
        function start(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ start: "start" });
        function start(args) {
            //handle the event
        }
    </script> 



{% endhighlight %}



### stop
{:#events:stop} 

Event triggers while user stopped sliding to change new value in RadialSlider.

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
Event parameters from RadialSlider<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the RadialSlider model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
number</td><td>
Returns the currently selected value after slide stop</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-change="change"></div>

    <script>
        function change(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <br />
        <p>
            Syncfusion is the enterprise technology partner of choice for Windows development
        </p>
    </div>
    <div id="defaultradialslider"></div>

    <script>
        $("#defaultradialslider").ejmRadialSlider({ stop: "stop" });
        function stop(args) {
            //handle the event
        }
    </script> 



{% endhighlight %}




