---
layout: post
title: ejmTimePicker | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmTimePicker
platform: Mobilejs
control: ejmTimePicker
documentation: API
keywords: ejmTimePicker, API, Essential Studio JS TimePicker (Mobile) 
---

# ejmTimePicker

The Essential JavaScript Mobile TimePicker provides support to display the TimePicker element within your web page and allows you to pick the time.

Custom Design for HTML TimePicker control.

$(element).ejmTimePicker()


#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input id="timepicker" data-role="ejmtimepicker" />    



{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

* module:ej.mobile.dialog

* module:ej.mobile.scrollpanel

* module:ej.mobile.scrollbar

## Members

### cssClass `String`
{:#members:cssclass}

Sets the root class for TimePicker theme. This cssClass API helps to use custom skinning option for TimePicker control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* ””

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-cssclass="customclass" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="timepicker" />
    <script>
        $(function () {	
            $("#timepicker").ejmTimePicker({ cssClass: "customclass" });
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
    <input id="timepicker" data-role="ejmtimepicker" data-ej-enabled=false />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="timepicker" data-role="none" />

    <script>
        $(function () {
            $("#timepicker").ejmTimePicker({ enabled: false });
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
    <input id="timepicker" data-role="ejmtimepicker" data-ej-enablepersistence=true />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="timepicker" data-role="none" />
    <script>
        $(function () {
            $("#timepicker").ejmTimePicker({ enablePersistence: true });
        });
    </script>


{% endhighlight %}

### hourFormat `String`
{:#members:hourformat}

Specifies the hour format.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-hourformat="twentyfour" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="timepicker" data-role="none" />

    <script>
        $(function () {
            $("#timepicker").ejmTimePicker({ hourFormat: "twentyfour" });
        });
    </script>


{% endhighlight %}


### locale `String`
{:#members:locale}

Change the TimePicker format based on given culture.

#### Default Value:

* “en-US”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-locale="en-US" />


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <input id="timepicker" data-role="none" />

    <script>
        $(function () {
            $("#timepicker").ejmTimePicker({ locale: "en-US" });
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
    <input id="timepicker" data-role="ejmtimepicker" data-ej-rendermode="android" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="timepicker" data-role="none" />
    <script>
        $(function () {
            $("#timepicker").ejmTimePicker({ renderMode: "android" });
        });
    </script>


{% endhighlight %}

### timeFormat `String`
{:#members:timeformat}

Specifies the time format.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-hourformat="twelve" data-ej-timeformat="hh:mm tt" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="timepicker" data-role="none" />
    <script>
        $(function () {
            $("#timepicker").ejmTimePicker({ hourFormat: "twelve", timeFormat: "hh:mm tt" });
        });
    </script>


{% endhighlight %}




### value `String`
{:#members:value}

Specifies the value.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-value="02:20 PM" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="timepicker" data-role="none" />
    <script>
        $(function () {
            $("#timepicker").ejmTimePicker({ value: "02:20 PM" });
        });
    </script>


{% endhighlight %}


## Methods

### disable()
{:#methods:disable}

To disable the timepicker control.

#### Example

{% highlight html %}

<input id="timepicker" data-role="ejmtimepicker" />
    <script>
        // changes the TimePicker current state to disabled
        $(function () {
            $("#timepicker").ejmTimePicker("disable");
        });
    </script>


{% endhighlight %}


### enable()
{:#methods:enable}

To enable the timepicker control.

#### Example

{% highlight html %}

<input id="timepicker" data-role="ejmtimepicker" />
    <script>
        $(function () {
            // change the TimePicker current state to enabled
            $("#timepicker").ejmTimePicker("enable");
        });
    </script>


{% endhighlight %}



### getValue()
{:#methods:getvalue}

Get the current value.

#### Example

{% highlight html %}

    <input id="timepicker" data-role="ejmtimepicker" />
    <script>
        // get the TimePicker current value
        $(function () {
            $("#timepicker").ejmTimePicker("getValue");
        });
    </script>


{% endhighlight %}

### hide()
{:#methods:hide}

To hide the TimePicker control

#### Example

{% highlight html %}

   <input id="timepicker" data-role="ejmtimepicker" />
    <script>
        $(function () {
            $("#timepicker").ejmTimePicker("hide");
        });
    </script>


{% endhighlight %}



### setCurrentTime()
{:#methods:setcurrenttime}

Set the given time

#### Example

{% highlight html %}

   <input id="timepicker" data-role="ejmtimepicker" />
    <script>
        // get the TimePicker current value
        $(function () {
            $("#timepicker").ejmTimePicker("setCurrentTime", "05:20");
        });
    </script>


{% endhighlight %}



### show()
{:#methods:show}

To show the TimePicker control

#### Example

{% highlight html %}

  <input id="timepicker" data-role="ejmtimepicker" />
    <script>
        $(function () {
            $("#timepicker").ejmTimePicker("show");
        });
    </script>


{% endhighlight %}


## Events



### change
{:#events:change}

Event triggers when the value is changed while interaction.

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
Event parameters from timepicker<table><br><tr><br><th>
<b>Name</b></th><th>
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
object</td><td>
returns the timepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the timepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-change="change" />
    <script>
        function change() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="timepicker" data-role="none" />
    <script>
        //change event for TimePicker
        $("#timepicker").ejmTimePicker({
            change: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}



### close
{:#events:close}

Event triggers when the control is closed after interaction.

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
Event parameters from timepicker<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the timepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Returns the timepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-close="close" />
    <script>
        function close() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="timepicker" data-role="none" />
    <script>
        //close event for TimePicker
        $("#timepicker").ejmTimePicker({
            close: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}




### focusIn
{:#events:focusin}

Event triggers when the input element is focused.

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
Event parameters from timepicker<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the timepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Returns the timepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-focusin="focusin" />
    <script>
        function focusin() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="timepicker" data-role="none" />
    <script>
        //focusIn event for TimePicker
        $("#timepicker").ejmTimePicker({
            focusIn: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}




### focusOut
{:#events:focusout}

Event triggers when the input element is focused out or blurred.

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
Event parameters from TimePicker<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the timepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Return the timepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-focusout="focusout" />
    <script>
        function focusout() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="timepicker" data-role="none" />
    <script>
        //focusOut event for TimePicker
        $("#timepicker").ejmTimePicker({
            focusOut: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}



### load
{:#events:load}

Event triggers when the control is loaded.

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
Event parameters from timepicker<table><br><tr><br><th>
<b>Name</b></th><th>
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
object</td><td>
returns the timepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the timepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-load="load" />
    <script>
        function load() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="timepicker" data-role="none" />
    <script>
        //load event for TimePicker
        $("#timepicker").ejmTimePicker({
            load: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}

### open
{:#events:open}

Event triggers when the control is opened for selection.

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
Event parameters from timepicker<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the timepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Returns the timepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-open="open" />
    <script>
        function open() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="timepicker" data-role="none" />
    <script>
        //open event for TimePicker
        $("#timepicker").ejmTimePicker({
            open: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}


### select
{:#events:select}

Event triggers when time value is selected.

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
Event parameters from TimePicker<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the timepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Returns the timepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="timepicker" data-role="ejmtimepicker" data-ej-select="select" />
    <script>
        function select() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="timepicker" data-role="none" />
    <script>
        //select event for TimePicker
        $("#timepicker").ejmTimePicker({
            select: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}


















