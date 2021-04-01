---
layout: post
title: ejmToggleButton | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmToggleButton
platform: Mobilejs
control: ejmToggleButton
documentation: API
keywords: ejmToggleButton, API, Essential Studio JS ToggleButton (Mobile)
---

## ejmToggleButton

The Essential JavaScript Mobile Toggle Button widget allows you to perform the toggle option by using checked and unchecked state. 

Custom Design for HTML ToggleButton control.

$(element).ejmToggleButton()

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton();
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

### cssClass `string`
{:#members:cssClass} 

Sets the root class for ToggleButton. This cssClass API helps to use custom skinning option for ToggleButton control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-cssclass="customclass"></div>

    <style>
        .customclass .e-m-tslider {
            background-color: red !important;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ cssClass: "customclass" });
    </script>

    <style>
        .customclass .e-m-tslider {
            background-color: red !important;
        }
    </style>



{% endhighlight %}



### enabled `boolean`
{:#members:enabled} 

Specifies whether to enable or disable the control.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-enabled="false"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ enabled: false });
    </script>



{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablePersistence} 

Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-enablepersistence="customclass"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ enablePersistence: true });
    </script>



{% endhighlight %}



### renderMode `enum`
{:#members:renderMode} 

Specifies the rendering mode of the control. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-rendermode="android"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ renderMode: "android" });
    </script>



{% endhighlight %}



### toggleState `boolean`
{:#members:toggleState} 

Specifies whether state of toggle button is on or off.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-togglestate="false"></div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ toggleState: false });
    </script>



{% endhighlight %}



## Methods

### disable()
{:#methods:disable} 

To disable the togglebutton.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable" data-ej-touchend="disable" />
    <br />
    <div id="togglebutton" data-role="ejmtogglebutton"></div>

    <script>
        function disable() {
            $("#togglebutton").ejmToggleButton("disable");
        }
    </script>



{% endhighlight %}



### enable()
{:#methods:enable} 

To enable the togglebutton.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable" data-ej-touchend="disable" />
    <input data-role="ejmbutton" type="button" data-ej-text="Enable" data-ej-touchend="enable" />
    <br />
    <div id="togglebutton" data-role="ejmtogglebutton"></div>

    <script>
        function disable() {
            $("#togglebutton").ejmToggleButton("disable");
        }
        function enable() {
            $("#togglebutton").ejmToggleButton("enable");
        }
    </script>



{% endhighlight %}



## Events

### change
{:#events:change} 

Event triggers when the state change occurs.

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
Event parameters from togglebutton.<table><br><tr><br><th><b>Name</b></th><th>
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
state</td><td>
boolean</td><td>
Returns the current state of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-change="change"></div>
    <script>
        function change(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ change: "change" });
        function change(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### touchEnd
{:#events:touchEnd} 

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
Event parameters from togglebutton.<table><br><tr><br><th><b>Name</b></th><th>
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
state</td><td>
boolean</td><td>
Returns the current state of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-touchend="touchend"></div>
    <script>
        function touchend(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ touchend: "touchend" });
        function touchend(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### touchStart
{:#events:touchStart} 

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
Event parameters from togglebutton.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise false.</td></tr>
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
state</td><td>
boolean</td><td>
Returns the current state of the control.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="togglebutton" data-role="ejmtogglebutton" data-ej-touchstart="touchstart"></div>
    <script>
        function touchstart(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="togglebutton"></div>
    <script>
        $("#togglebutton").ejmToggleButton({ touchstart: "touchstart" });
        function touchstart(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



