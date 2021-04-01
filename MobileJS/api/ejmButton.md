---
layout: post
title: ejmButton | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmButton
platform: Mobilejs
control: ejmButton
documentation: API
keywords: ejmButton, API, Essential Studio JS Button (Mobile)
---

# ejmButton

Custom Design for HTML Button control.

$(element).ejmButton();

#### Example

**Button:**

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input id="button" type="button" />

    <script>

        $("#button").ejmButton();
    </script>


{% endhighlight %}

**ActionLink:**



{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <a id="button" data-role="ejmactionlink" ></a>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <a id="button"></a>

    <script>

        $("#button").ejmActionLink();
    </script>


{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.touch

## Members

### color
{:#members:color} 

Section for color specific functionalities.

### color.border `string`
{:#members:color-border} 

Specifies the color border to Button outer border.

#### Default value

* “”

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-color-border="red" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <input id="button" type="button" />
    <script>
        $("#button").ejmButton({ color: { border: "red" } })
    </script>


{% endhighlight %}

### color.fill `string`
{:#members:color-fill} 

Specifies the color fill to Button background color.

#### Default value

* “”

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-color-fill="red" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering --> 
    <input id="button" type="button" />
    <script>
        $("#button").ejmButton({ color: { fill: "red" } })
    </script>


{% endhighlight %}

### color.text `string`
{:#members:color-text} 

Specifies the color text to Button text

#### Default value

* “”

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-color-text="red" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input id="button" type="button" />

    <script>
        $("#button").ejmButton({ color: { text: "red" } })
    </script>


{% endhighlight %}

### contentType `enum`
{:#members:contenttype} 

Specifies the contentType of the Button. See [ButtonContentType](http://help.syncfusion.com/mobilejs/api/global#buttoncontenttype)

#### Default Value

* ej.mobile.Button.ContentType.Text



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <button id="button1" type="button" data-role="ejmbutton" data-ej-contenttype="image" data-ej-imageclass="e-m-icon-settings"></button>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <button id="button1" type="button"></button>

    <script>

        $("#button1").ejmButton({ contentType: ej.mobile.Button.ContentType.Image, imageClass: "e-m-icon-settings" });

    </script>



{% endhighlight %}

### cssClass `string`
{:#members:cssclass} 

The root class for the Button widget to customize the existing theme

#### Default value

“”

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <style>
        .customize {
            width: 300px;
        }
    </style>
    <input id="button" type="button" data-role="ejmbutton" data-ej-cssclass="customize" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering --> 

    <style>
        .customize {
            width: 300px;
        }
    </style>
    <input id="button" type="button" />
    <script>
        $("#button").ejmButton({ cssClass: "customize" })
    </script>


{% endhighlight %}

### enabled `boolean`
{:#members:enabled} 

Specifies whether to enable or disable the control.

#### Default value

* true

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-enabled="false" />


{% endhighlight %}





{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <input id="button" type="button"/>
    <script>

        $("#button").ejmButton({ enabled: false })
    </script>


{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence} 

Allows the current model values to be saved in local storage or browser cookies for state maintenance when it is set to true. While refreshing the page, it retains the model value from browser cookies or local storage.

N> [Local storage](http://www.w3schools.com/html/html5_webstorage.asp) is supported only in Html5 supported browsers. If the browsers don’t have support for local storage, browser cookies will be used to maintain the state.

#### Default value

* false



#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->

    <input id="button" type="button" data-role="ejmbutton" data-ej-enablepersistence="true" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <input type="button" id="button" />

    <script>

        $("#button").ejmButton({ enablePersistence: true });

    </script>


{% endhighlight %}

### enableRippleEffect `boolean`
{:#members:enablerippleeffect} 

Specifies whether to enable or disable ripple effect.

#### Default value

* false

#### Example

{% highlight html %}

   <!-- Unobtrusive way of rendering -->

    <div style="width:auto;height:auto;position:absolute;">
        <input id="button" type="button" data-role="ejmbutton" data-ej-enablerippleeffect="true" />
    </div>


{% endhighlight %}





{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <div style="width:auto;height:auto;position:absolute;">
        <input id="button" type="button" />
    </div>
    <script>

        $("#button").ejmButton({ enableRippleEffect: true })
    </script>


{% endhighlight %}

### href `string`
{:#members:href} 

Specifies the href of action link Button

N> This property is only applicable to ejmActionLink

#### Default value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <a id="button" data-role="ejmactionlink" data-ej-text="MicroSoft" data-ej-href="https://www.microsoft.com"></a>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <a id="button"></a>

    <script>
        $("#button").ejmActionlink({ href: "https://www.microsoft.com", text: "MicroSoft" })
    </script>


{% endhighlight %}

### imageClass `string`
{:#members:imageclass} 

Specifies the css class of image.

N> This property is only applicable when Button control is render with HTML button tag.

#### Default value

* null

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <button id="button" data-role="ejmbutton" data-ej-contenttype="image" data-ej-imageclass="e-m-icon-settings"></button>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <button id="button"></button>

    <script>
        $("#button").ejmButton({ contentType: ej.mobile.Button.ContentType.Image, imageClass: "e-m-icon-settings" })
    </script>


{% endhighlight %}

### imagePosition `enum`
{:#members:imageposition} 

Specifies the position of image. See [ButtonImagePosition](http://help.syncfusion.com/mobilejs/api/global#buttonimageposition)


N> This property is only applicable when render the Button control with HTML button tag and contentType property set as “both”

#### Default value

* ej.mobile.Button.ImagePosition.Left

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->

    <style>
        .chat {
            background-image: url(chat.png);
        }
    </style>

    <button id="button" data-role="ejmbutton" data-ej-contenttype="both" data-ej-imageclass="chat" data-ej-imageposition="right"></button>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <style>
        .chat {
            background-image: url(chat.png);
        }
    </style>

    <button id="button"></button>

    <script>
        $("#button").ejmButton({ contentType: ej.mobile.Button.ContentType.Both, imageClass: "chat",imagePosition:ej.mobile.Button.ImagePosition.Right })
    </script>


{% endhighlight %}

### locale `string`
{:#members:locale} 

Set the localization culture for Button Widget.

#### Default value

* “en-US”

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-locale="en-US" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <input id="button" type="button" />
    <script>
        $("#button").ejmButton({ locale: "en-US" })
    </script>



{% endhighlight %}

### renderMode `enum`
{:#members:rendermode} 

Specifies the rendering mode of the control. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default value

* auto

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" />
    <script>

        $("#button").ejmButton({ renderMode: "android" })
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <input id="button" type="button" data-role="ejmbutton" data-ej-rendermode="android" />


{% endhighlight %}

### showBorder `boolean`
{:#members:showborder} 

Displays the Button with outer border.

#### Default value

* true

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-showborder="false" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input id="button" type="button" />

    <script>

        $("#button").ejmButton({ showBorder: false })
    </script>


{% endhighlight %}

### style `enum`
{:#members:style} 

Specifies the style of the control. See [ButtonStyle](http://help.syncfusion.com/mobilejs/api/global#buttonstyle)


#### Default value

* normal

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" />
    <script>
        $("#button").ejmButton({ style: "large" })
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-style="large" />


{% endhighlight %}

### text `string`
{:#members:text} 

Specifies the text to Button

#### Default value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-text="Download"/>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->

    <input id="button" type="button" />
    <script>

        $("#button").ejmButton({ text: "Download" })
    </script>


{% endhighlight %}

## Methods

### disable()
{:#methods:disable}

To disable the button.

#### Example

{% highlight html %}

    <input id="button" type="button" data-role="ejmbutton" />

    <script>

        $(function () {

            var button = $("#button").data("ejmButton");

            button.disable(); 

        });

    </script>


{% endhighlight %}



{% highlight html %}

        <input id="button" type="button" data-role="ejmbutton" />

    <script>

        $(function () {

            var button = $("#button").ejmButton("disable"); 

        });

    </script>


{% endhighlight %}



### enable()
{:#methods:enable}

To enable the Button.

#### Example



{% highlight html %}

    <input id="button" type="button" data-role="ejmbutton"  />

    <script>

        $(function () {

            var button = $("#button").data("ejmButton");

            button.enable(); 

        });

    </script>


{% endhighlight %}



{% highlight html %}

    
    <input id="button" type="button" data-role="ejmbutton" />

    <script>

        $(function () {

            var button = $("#button").ejmButton("enable"); 

        });

    </script>


{% endhighlight %}

## Events

### touchEnd
{:#events:touchend}

Event triggers when touch end happens on the control.

<table>
<tr>
<td>
Name </td><td>
Type</td><td>
Description</td></tr>
<tr>
<td>
arguments</td><td>
object</td><td>
Event parameters from Button.<table><br><tr><br><td>Name</td><td>
Type</td><td>
Description</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the Button model.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
<br>Returns the name of the event.</td></tr>
<tr>
<td>
status</td><td>
boolean</td><td>
Returns the Button state.</td></tr>
</table>


</td></tr>
</table>


#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-touchend="touchend" />

    <script>
        
        function touchend(args) {
            //handle the event
        }

    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input id="button" type="button" />

    <script>

        $("#button").ejmButton({

            touchEnd: function (args) {
                //handling the event
            }

        });

    </script>


{% endhighlight %}

### touchStart
{:#events:touchstart}

Event triggers when touch start happens on the control.

<table>
<tr>
<td>
Name </td><td>
Type</td><td>
Description</td></tr>
<tr>
<td>
arguments</td><td>
object</td><td>
Event parameters from Button.<table><br><tr><br><td>Name</td><td>
Type</td><td>
Description</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
If the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
object</td><td>
Returns the Button model.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
<br>Returns the name of the event.</td></tr>
<tr>
<td>
status</td><td>
boolean</td><td>
Returns the Button state.</td></tr>
</table>


</td></tr>
</table>


#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="button" type="button" data-role="ejmbutton" data-ej-touchstart="touchstart" />
    <script>
        function touchstart(args) {
            //handle the event
        }
    </script>

{% endhighlight %}





{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input id="button" type="button" />

    <script>

        $("#button").ejmButton({

            touchEnd: function (args) {
                //handling the event
            }

        });
    </script>


{% endhighlight %}