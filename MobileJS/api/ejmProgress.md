---
layout: post
title: ejmProgress | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmProgress
platform: Mobilejs
control: ejmProgress
documentation: API
keywords: ejmProgress, API, Essential Studio JS ProgressBar (Mobile) 
---


# ejmProgress
The Essential JavaScript Mobile Progress Bar widget shows the progress of a lengthy operation by filling a rectangle with chunks from left to right

Custom Design for HTML ProgressBar control.

$(element).ejmProgress()


#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="progress" data-role="ejmprogress"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="progress"></div>
    <script>
        // Create progressbar
        $(function () {
            $("#progress").ejmProgress();
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


### enableCustomText `Boolean`
{:#members:enablecustomtext}

Specifies whether to accept custom text or not.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="progress" data-role="ejmprogress" data-ej-enablecustomtext=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        // Create progressbar
        $(function () {
            $("#progress").ejmProgress({ enableCustomText: false });
        });
    </script>


{% endhighlight %}


### enabled `Boolean`
{:#members:enabled}

Specifies whether the control is enabled or disabled.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="progress" data-role="ejmprogress" data-ej-enabled=true></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        // Create progressbar
        $(function () {
            $("#progress").ejmProgress({ enabled: false });
        });
    </script>


{% endhighlight %}



### enablePersistence `Boolean`
{:#members:enablepersistence}

Saves current model value to browser cookies for state maintenance. While refreshing the page it retains the model value and applies from browser cookies.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="progress" data-role="ejmprogress" data-ej-enablepersistence=false></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        // Create progressbar
        $(function () {
            $("#progress").ejmProgress({ enablePersistence: false });
        });
    </script>


{% endhighlight %}



### height `Int`
{:#members:height}

Specifies the height of the ProgrssBar control.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-height=10></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ height: 10 });
        });
    </script>


{% endhighlight %}



### incrementStep `Int`
{:#members:incrementstep}

Specifies the value to be added in each step of increment.

#### Default Value:

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-incrementstep=2></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ incrementStep: 2 });
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
    <div id="progress" data-role="ejmprogress" data-ej-maxvalue=90></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ maxValue: 90 });
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
    <div id="progress" data-role="ejmprogress" data-ej-minvalue=10></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ minValue: 10 });
        });
    </script>


{% endhighlight %}



### orientation `Enum`
{:#members:orientation}

Specifies the orientation whether it is horizontal or vertical. See[Orientation](http://help.syncfusion.com/mobilejs/api/global#members:orientation)

#### Default Value:

* ej.mobile.Progress.Orientation.Horizontal

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-orientation="horizontal"></div>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress();
            $("#progress").ejmProgress({ orientation: ej.mobile.Progress.Orientation.Horizontal });
        });
    </script>


{% endhighlight %}

### percentage `Int`
{:#members:percentage}

Specifies the initial value in percentage.

#### Default Value:

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-percentage=35></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ percentage: 35 });
        });
    </script>


{% endhighlight %}


### renderMode `Enum`
{:#members:rendermode}

Changes the rendering mode. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value:

* auto

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-rendermode="auto"></div>


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ renderMode: ej.mobile.RenderMode.Auto });
        });
    </script>


{% endhighlight %}


### text `String`
{:#members:text}

Specifies the ProgressBar text

#### Default Value:

* “”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-enablecustomtext="true" data-ej-text="Loading..."></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ enableCustomText: true, text: "Loading..." });
        });
    </script>


{% endhighlight %}


### value `Int`
{:#members:value}

Specifies the initial value.

#### Default Value:

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-value=35></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ value: 35 });
        });
    </script>


{% endhighlight %}




### width `Int`
{:#members:width}

Specifies the width of the ProgressBar control.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="progress" data-role="ejmprogress" data-ej-width=350></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({ width: 350 });
        });
    </script>


{% endhighlight %}



## Methods


### getPercentage()
{:#methods:getpercentage}

Get current value of the ProgressBar in percentage.

#### Example

{% highlight html %}

<div id="progress" data-role="ejmprogress"></div>
    <script>
        // Get the current percent value
        $(function () {
            $("#progress").ejmProgress("getPercentage");
        });
    </script>


{% endhighlight %}


### getValue()
{:#methods:getvalue}

Gets the currentvalue of the ProgressBar.

#### Example

{% highlight html %}

<div id="progress" data-role="ejmprogress"></div>
    <script>
        // Get the current value
        $(function () {
            $("#progress").ejmProgress("getValue");
        });
    </script>


{% endhighlight %}




### setCustomText()
{:#methods:setcustomtext}

Set the custom text on each action complete.

#### Example

{% highlight html %}

<div id="progress" data-role="ejmprogress"></div>
    <script>
        // Set the custom text
        $(function () {
            $("#progress").ejmProgress("setCustomText", "Downloading..");
        });
    </script>


{% endhighlight %}




## Events


### change
{:#events:change}

Event triggers when the ProgressBar value changes. 

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
event parameters from ProgressBar<table><br><tr><br><th>
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
string</td><td>
Returns the progressbar model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
percentage</td><td>
int</td><td>
Returns the current element associated percentage</td></tr>
<tr>
<td>
value</td><td>
int</td><td>
Returns the current element associated value</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the progressbar current text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
<div id="progress" data-role="ejmprogress" data-ej-change="onChange"></div>
    <script>
        // change event
        function onChange(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({
                change: function (args) { //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### complete
{:#events:complete}

Event triggers when it reaches the maximum value.

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
event parameters from progressbar<table><br><tr><br><th>
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
string</td><td>
returns the progressbar model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
percentage</td><td>
int</td><td>
returns the current element associated percentage</td></tr>
<tr>
<td>
value</td><td>
int</td><td>
returns the current element associated value</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
returns the progressbar current text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
<div id="progress" data-role="ejmprogress" data-ej-complete="onComplete"></div>
    <script>
        // complete event
        function onComplete(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
<div id="progress"></div>
    <script>
        //complete event
        $(function () {
            $("#progress").ejmProgress({
                complete: function (args) { //handle the event
                }
            });
        });
    </script>


{% endhighlight %}




### create
{:#events:create}

Event triggers when the progressbar is created.

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
event parameters from progressbar<table><br><tr><br><th>
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
string</td><td>
Returns the progressbar model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
  <div id="progress" data-role="ejmprogress" data-ej-create="onCreate"></div>
    <script>
        // Create event
        function onCreate(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({
                create: function (args) { //handle the event
                }
            });
        });
    </script>


{% endhighlight %}


### start
{:#events:start}

Event triggers when progress started. 

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
event parameters from progressbar<table><br><tr><br><th>
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
string</td><td>
Returns the progressbar model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
percentage</td><td>
int</td><td>
Returns the current element associated percentage</td></tr>
<tr>
<td>
value</td><td>
int</td><td>
Returns the current element associated value</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
   <div id="progress" data-role="ejmprogress" data-ej-start="onStart"></div>
    <script>
        // start event
        function onStart(args) { //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <div id="progress"></div>
    <script>
        $(function () {
            $("#progress").ejmProgress({
                start: function (args) { //handle the event
                }
            });
        });
    </script>


{% endhighlight %}




