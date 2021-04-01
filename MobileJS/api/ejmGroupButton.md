---
layout: post
title: ejmGroupButton | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmGroupButton
platform: Mobilejs
control: ejmGroupButton
documentation: API
keywords: ejmGroupButton, API, Essential Studio JS GroupButton (Mobile)
---

# ejmGroupButton

The Essential JavaScript Mobile GroupButton widget helps to display multiple buttons that stack together in a single line and appear as a navigation component.

Custom Design for HTML GroupButton control.

$(element).ejmGroupButton()

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering with radio buttons -->    
    <div data-role="ejmgroupbutton">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Unobtrusive way of rendering with checkboxes -->
    <div data-role="ejmgroupbutton">
        <label>
            <input type="checkbox" name="options">
            iPod
        </label>
        <label>
            <input type="checkbox" name="options">
            iPad
        </label>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Unobtrusive way of rendering with buttons -->
    <div data-role="ejmgroupbutton">
        <button>iPod</button>
        <button>iPad</button>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering with radio buttons -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton();
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering with checkboxes -->
    <div data-role="ejmgroupbutton">
        <label>
            <input type="checkbox" name="options">
            iPod
        </label>
        <label>
            <input type="checkbox" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton();
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering with buttons -->
    <div data-role="ejmgroupbutton">
        <button>iPod</button>
        <button>iPad</button>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton();
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
{:#members:cssclass} 

Sets the root class for GroupButton theme. This cssClass API helps to use custom skinning option for GroupButton control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div data-role="ejmgroupbutton" data-ej-cssclass="customclass">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <style>
        .customclass * {
            color: red;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton({ cssClass: "customclass" });
    </script>

    <style>
        .customclass * {
            color: red;
        }
    </style>



{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence}
 
Current model value to browser cookies for state maintenance. While refreshing the page, the model value applied from browser cookies retains.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->    
    <div data-role="ejmgroupbutton" data-ej-enablepersistence="true">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton({ cssClass: "customclass" });
    </script>



{% endhighlight %}



### items `string`
{:#members:items}

Renders the GroupButton using data source which contains array of items.

#### Default Value

* []

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->    
    <div data-role="ejmgroupbutton" data-ej-items="[{ text: 'iPod' }, { text: 'iPad' }]">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn" data-role="ejmgroupbutton"></div>

    <script>
        $("#grpbtn").ejmGroupButton({ items: [{ text: "iPod" }, { text: "iPad" }] });
    </script>



{% endhighlight %}



### renderMode `enum`
{:#members:rendermode}

Changes the rendering mode of the GroupButton. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div data-role="ejmgroupbutton" data-ej-rendermode="android">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton({ renderMode: "android" });
    </script>




{% endhighlight %}



### selectedItemIndex `number`
{:#members:selecteditemindex}

Specifies the item which one is to be selected initially.

#### Default Value

* 0

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div data-role="ejmgroupbutton" data-ej-selecteditemindex="1">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton({ selectedItemIndex: 1 });
    </script>




{% endhighlight %}



## Events


### select
{:#events:select}

Event triggers when the select happens in the GroupButton

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
Event parameters from GroupButton<table><br><tr><br><th><b>Name</b></th><th>
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
boolean</td><td>
Returns the GroupButton model</td></tr>
<tr>
<td>
type</td><td>
boolean</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
text</td><td>
boolean</td><td>
Returns the current button text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="grpbtn" data-role="ejmgroupbutton" data-ej-select="select">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        function select(args) { //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton({ select: "select" });
        function select(args) { //handle the event
        }
    </script>




{% endhighlight %}


### touchEnd
{:#events:touchend}

Event triggers when the touchend happens in the GroupButton

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
Event parameters from GroupButton<table><br><tr><br><th><b>Name</b></th><th>
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
boolean</td><td>
Returns the GroupButton model</td></tr>
<tr>
<td>
type</td><td>
boolean</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
text</td><td>
boolean</td><td>
Returns the selected button text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="grpbtn" data-role="ejmgroupbutton" data-ej-touchend="touchend">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        function touchend(args) { //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton({ touchEnd: "touchend" });
        function touchend(args) { //handle the event
        }
    </script>




{% endhighlight %}



### touchStart
{:#events:touchstart}

Event triggers when the touchstart happens in the GroupButton

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
Event parameters from GroupButton<table><br><tr><br><th><b>Name</b></th><th>
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
boolean</td><td>
Returns the GroupButton model</td></tr>
<tr>
<td>
type</td><td>
boolean</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
text</td><td>
boolean</td><td>
Returns the current button text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="grpbtn" data-role="ejmgroupbutton" data-ej-touchstart="touchstart">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        function touchstart(args) { //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="grpbtn">
        <label>
            <input type="radio" name="options">
            iPod
        </label>
        <label>
            <input type="radio" name="options">
            iPad
        </label>
    </div>

    <script>
        $("#grpbtn").ejmGroupButton({ touchStart: "touchstart" });
        function touchstart(args) { //handle the event
        }
    </script>




{% endhighlight %}



