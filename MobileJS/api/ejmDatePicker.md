---
layout: post
title: ejmDatePicker | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmDatePicker
platform: Mobilejs
control: ejmDatePicker
documentation: API
keywords: ejmDatePicker, API, Essential Studio JS DatePicker (Mobile) 
---

# ejmDatePicker

It displays the date picker element within your web page and allows you to pick the date. 

Custom Design for Html DatePicker control.

$(element).ejmDatePicker()


#### Example

{% highlight html %}


<!-- Unobtrusive way of rendering -->
<input id="datepicker" data-role="ejmdatepicker" />    



{% endhighlight %}



### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

* module:ej.mobile.menu

* module:ej.mobile.navigationbar

* module:ej.mobile.dialog

* module:ej.mobile.button

* module:ej.mobile.scrollpanel

* module:ej.mobile.scrollbar

## Members

### cssClass `String`
{:#members:cssclass}

Sets the root class for DatePicker theme. This cssClass API helps to use custom skinning option for DatePicker control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* ””

#### Example

{% highlight html %}


<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-cssclass="customclass" />



{% endhighlight %}



{% highlight html %}


 <!-- Obtrusive way of rendering -->
    <input id="datepicker" />
    <script>
        $(function () {	
            $("#datepicker").ejmDatePicker({ cssClass: "customclass" });
        });
    </script>



{% endhighlight %}


### dateFormat `String`
{:#members:dateformat}

Specifies the date format.

#### Default Value:

* null

#### Example

{% highlight html %}


<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-dateformat="MMMM dd, yyyy" />



{% endhighlight %}



{% highlight html %}


<!-- Obtrusive way of rendering -->
    <input id="datepicker" data-role="none" />

    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ dateFormat: "MMMM dd, yyyy" });
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
    <input id="datepicker" data-role="ejmdatepicker" data-ej-enabled=false />



{% endhighlight %}



{% highlight html %}


<!-- Obtrusive way of rendering -->
    <input id="datepicker" data-role="none" />

    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ enabled: false });
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
    <input id="datepicker" data-role="ejmdatepicker" data-ej-enablepersistence=true />



{% endhighlight %}



{% highlight html %}


<!-- Obtrusive way of rendering -->
    <input id="datepicker" data-role="none" />
    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ enablePersistence: true });
        });
    </script>



{% endhighlight %}

### locale `String`
{:#members:locale}

Change the DatePicker format based on given culture.

#### Default Value:

* “en-US”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-locale="en-US" />


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <input id="datepicker" data-role="none" />

    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ locale: "en-US" });
        });
    </script>


{% endhighlight %}


### maxDate `String`
{:#members:maxdate}

Specifies the maximum selectable date.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-maxdate="12/31/2030" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="datepicker" data-role="none" />
    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ maxDate: "12/31/2030" });
        });
    </script>


{% endhighlight %}


### minDate `String`
{:#members:mindate}

Specifies the minimum selectable date.

#### Default Value:

* null

#### Example

{% highlight html %}


<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-mindate="01/01/2000" />



{% endhighlight %}



{% highlight html %}


<!-- Obtrusive way of rendering -->
    <input id="datepicker" data-role="none" />

    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ minDate: "01/01/2000" });
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
    <input id="datepicker" type="date" data-role="ejmdatepicker" data-ej-rendermode="android" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="datepicker" type="date" />

    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ renderMode: "android" });
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
    <input id="datepicker" data-role="ejmdatepicker" data-ej-value="04/23/2010" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="datepicker" data-role="none" />
    <script>
        $(function () {
            $("#datepicker").ejmDatePicker({ value: "04/23/2010" });
        });
    </script>


{% endhighlight %}



## Methods

### disable()
{:#methods:disable}

To disable the datepicker

#### Example

{% highlight html %}

<input id="datepicker" data-role="ejmdatepicker" />
    <script>
        // changes the DatePicker current state to disabled
        $(function () {
            $("#datepicker").ejmDatePicker("disable");
        });
    </script>


{% endhighlight %}


### enable()
{:#methods:enable}

To enable the datepicker

#### Example

{% highlight html %}

<input id="datepicker" data-role="ejmdatepicker" />
    <script>
        $(function () {
            // change the DatePicker current state to enabled
            $("#datepicker").ejmDatePicker("enable");
        });
    </script>


{% endhighlight %}



### getValue()
{:#methods:getvalue}

Get the current value.

#### Example

{% highlight html %}

    <input id="datepicker" data-role="ejmdatepicker" />
    <script>
        // get the DatePicker current value
        $(function () {
            $("#datepicker").ejmDatePicker("getValue");
        });
    </script>


{% endhighlight %}


### hide()
{:#methods:hide}

To hide the DatePicker control

#### Example

{% highlight html %}

   <input id="datepicker" data-role="ejmdatepicker" />
    <script>
        $(function () {
            $("#datepicker").ejmDatePicker("hide");
        });
    </script>


{% endhighlight %}




### setCurrentDate()
{:#methods:setcurrentdate}

Set the given date.

#### Example

{% highlight html %}

<input id="datepicker" data-role="ejmdatepicker" />
    <script>
        // get the DatePicker current value
        $(function () {
            $("#datepicker").ejmDatePicker("setCurrentDate", "12/31/2000");
        });
    </script>


{% endhighlight %}

### show()
{:#methods:show}

To show the DatePicker control

#### Example

{% highlight html %}

  <input id="datepicker" data-role="ejmdatepicker" />
    <script>
        $(function () {
            $("#datepicker").ejmDatePicker("show");
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
Event parameters from datepicker<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set true when the event should be canceled, otherwise false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the DatePicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the DatePicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-change="change" />
    <script>
        function change() {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


<!-- Obtrusive way of rendering -->
<input id="datepicker" data-role="none" />
    <script>
        //change event for DatePicker
        $("#datepicker").ejmDatePicker({
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
Event parameters from DatePicker<table><br><tr><br><th>
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
object</td><td>
Returns the datepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the datepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-close="close" />
    <script>
        function close() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="datepicker" data-role="none" />
    <script>
        //close event for DatePicker
        $("#datepicker").ejmDatePicker({
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
Event parameters from datepicker<table><br><tr><br><th>
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
object</td><td>
Returns the datepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the datepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-focusin="focusin" />
    <script>
        function focusin() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="datepicker" data-role="none" />
    <script>
        //focusIn event for DatePicker
        $("#datepicker").ejmDatePicker({
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
Event parameters from datepicker<table><br><tr><br><th>
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
object</td><td>
Returns the datepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the datepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-focusout="focusout" />
    <script>
        function focusout() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="datepicker" data-role="none" />
    <script>
        //focusOut event for DatePicker
        $("#datepicker").ejmDatePicker({
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
Event parameters from datepicker<table><br><tr><br><th>
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
object</td><td>
Returns the datepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the datepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-load="load" />
    <script>
        function load() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="datepicker" data-role="none" />
    <script>
        //load event for DatePicker
        $("#datepicker").ejmDatePicker({
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
Event parameters from datepicker<table><br><tr><br><th>
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
object</td><td>
Returns the datepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the datepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-open="open" />
    <script>
        function open() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="datepicker" data-role="none" />
    <script>
        //open event for DatePicker
        $("#datepicker").ejmDatePicker({
            open: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}


### select
{:#events:select}

Event triggers when date value is selected.

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
Event parameters from datepicker<table><br><tr><br><th>
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
object</td><td>
Returns the datepicker model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
return the datepicker value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="datepicker" data-role="ejmdatepicker" data-ej-select="select" />
    <script>
        function select() {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="datepicker" data-role="none" />
    <script>
        //select event for DatePicker
        $("#datepicker").ejmDatePicker({
            select: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}




































