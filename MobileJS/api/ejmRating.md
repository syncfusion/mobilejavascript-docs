---
layout: post
title: ejmRating | API Reference | Mobile JS | Syncfusion
description:
documentation: API
platform: Mobilejs
keywords: ejmRating, API, Essential Studio JS Rating (Mobile) 
---

# ejmRating

The Essential JavaScript Mobile Rating control lets you quickly set a value by selecting a number of symbols from a group.

Custom Design for HTML Rating control.

$(element).ejmRating();

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating"></div>

{% endhighlight %}

{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating();
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


### enabled `boolean`
{:#members:enabled}




Specifies whether to enable or disable the control.


#### Default Value



* true




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-enabled="false"></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ enabled: false });
    </script>


{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence}




Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.


#### Default Value



* false




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-enablepersistence="true"></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ enablePersistence: true });
    </script>

{% endhighlight %}


### incrementStep `int`
{:#members:incrementstep}




Specifies the step value for incrementation.


#### Default Value



* 1




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-incrementstep="1"></div>

{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering --> 
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ incrementStep: 1 });
    </script>
                           
{% endhighlight %}


### maxValue `int`
{:#members:maxvalue}




Specifies the maximum value of Rating.


#### Default Value



* 5




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-maxvalue="7"></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering --> 
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ maxValue: 7 });
    </script> 
    
{% endhighlight %}


### minValue `int`
{:#members:minvalue}




Specifies the minimum value.


#### Default Value



* 0




#### Example


{% highlight html %}
 
    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-minvalue="4"></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering --> 
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ minValue: 4 });
    </script> 
                 
{% endhighlight %}



### orientation `enum`
{:#members:orientation}




Specifies whether the orientation is horizontal or vertical. See [Orientation](http://help.syncfusion.com/mobilejs/api/global#ratingorientation)


#### Default Value



* "horizontal"




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-orientation="vertical"></div>

{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ orientation: "vertical" });
    </script>
    
{% endhighlight %}



### precision `enum`
{:#members:precision}




Specifies the precision value. See [Precision](http://help.syncfusion.com/mobilejs/api/global#ratingprecision)


#### Default Value



* "full"




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-precision="half"></div>

{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ precision: "half" });
    </script>  
            
{% endhighlight %}



### readOnly `boolean`
{:#members:readonly}




Specifies whether the control is read only.


#### Default Value



* false




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-readonly="true" ></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ readOnly: true });
    </script>
    
{% endhighlight %}


### renderMode `enum`
{:#members:rendermode}




Specifies the rendering mode of the control. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)


#### Default Value



* "auto"




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-rendermode="android"></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ renderMode: "android" });
    </script>
    
{% endhighlight %}



### shape `enum`
{:#members:shape}




Specifies the shape. See [Shape](http://help.syncfusion.com/mobilejs/api/global#ratingshape)


#### Default Value



* "star"




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-shape="circle"></div>

{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ shape: "circle" });
    </script>
    
{% endhighlight %}


### shapeHeight `int`
{:#members:shapeheight}




Specifies the shape height.


#### Default Value



* 25




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-shapeheight="40" ></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ shapeHeight: 40 });
    </script>
      
{% endhighlight %}


### shapeWidth `int`
{:#members:shapewidth}




Specifies the shape width.


#### Default Value



* 25




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-shapewidth="40" ></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ shapeWidth: 40 });
    </script>    
                
{% endhighlight %}


### spaceBetweenShapes `int`
{:#members:spacebetweenshapes}




Specifies the space between shapes.


#### Default Value



* 25




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-spacebetweenshapes="40" ></div>
    
{% endhighlight %}


{% highlight html %} 
    
    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({ spaceBetweenShapes: 40 });
    </script>     
                
{% endhighlight %}



### value `int`
{:#members:value}




Specifies the current value.


#### Default Value



* 1




#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-value="2"></div>
    
{% endhighlight %}


{% highlight html %} 

    <!-- Obtrusive way of rendering -->
    <div id="rating"></div>
    <script>

        $("#rating").ejmRating({ value: 2 });
    </script>
                     
{% endhighlight %}



## Methods




### disable()
{:#methods:disable}




To disable the Rating.



#### Example


{% highlight html %} 

    <input data-role="ejmbutton" type="button" data-ej-text="Disable" data-ej-touchend="disable" /><br />
    <div id="rating" data-role="ejmrating"></div>

    <script>
        function disable() {
            $("#rating").ejmRating("disable");
        }
    </script>

{% endhighlight %}



### enable()
{:#methods:enable}




To enable the rating.



#### Example


{% highlight html %} 

    <input data-role="ejmbutton" type="button" data-ej-text="Disable" data-ej-touchend="disable" />
    <input data-role="ejmbutton" type="button" data-ej-text="Enable" data-ej-touchend="enable" /><br />
        
    <div id="rating" data-role="ejmrating"></div>

    <script>
        function disable() {
            $("#rating").ejmRating("disable");
        }
        function enable() {
            $("#rating").ejmRating("enable");
        }        
    </script>

{% endhighlight %}


### getValue()
{:#methods:getvalue}




To get the current value.



#### Example


{% highlight html %} 

    <input data-role="ejmbutton" type="button" data-ej-text="Get Value" data-ej-touchend="get" /><br />

    <div id="rating" data-role="ejmrating"></div>

    <script>
        function get() {
            var value = $("#rating").ejmRating("getValue");
            alert("Current value is: " + value);
        }
    </script>

{% endhighlight %}


### hide()
{:#methods:hide}




To hide the Rating.



#### Example


{% highlight html %} 

    
    <input data-role="ejmbutton" type="button" data-ej-text="Hide" data-ej-touchend="hide" /><br />
        
    <div id="rating" data-role="ejmrating"></div>

    <script>
        function hide() {
            $("#rating").ejmRating("hide");
        }
    </script>

{% endhighlight %}


### reset()
{:#methods:reset}




To reset the value.



#### Example


{% highlight html %} 

    
    <input data-role="ejmbutton" type="button" data-ej-text="Reset" data-ej-touchend="reset" /><br />
        
    <div id="rating" data-role="ejmrating"></div>

    <script>
        function reset() {
            $("#rating").ejmRating("reset");
        }
    </script>

{% endhighlight %}

### setValue()
{:#methods:setvalue}




To set the value.



#### Example


{% highlight html %} 

    
    <input data-role="ejmbutton" type="button" data-ej-text="Set Value" data-ej-touchend="set" /><br />
        
    <div id="rating" data-role="ejmrating"></div>

    <script>
        function set() {
            $("#rating").ejmRating("setValue", 2);
        }
    </script>

{% endhighlight %}


### show()
{:#methods:show}




To show the Rating.



#### Example


{% highlight html %} 

    
    <input data-role="ejmbutton" type="button" data-ej-text="Hide" data-ej-touchend="hide" />
    <input data-role="ejmbutton" type="button" data-ej-text="Show" data-ej-touchend="show" /><br />
            
    <div id="rating" data-role="ejmrating"></div>

    <script>
        function hide() {
            $("#rating").ejmRating("hide");
        }            
        function show() {
            $("#rating").ejmRating("show");
        }
    </script>

{% endhighlight %}

## Events




### change
{:#events:change}




Event triggers when the value changed.

<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>argument</td>
<td>Object</span></td>
<td>Event parameters from Rating.
<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>cancel</td>
<td>boolean</span></td>
<td>returns true if the event should be cancelled; otherwise, false.</td>
</tr>
<tr>
<td>type</td>
<td>string</span></td>
<td>returns the name of the event.</td>
</tr>
<tr>
<td>model</td>
<td>Object</span></td>
<td>returns the model value of the control.</td>
</tr>
<tr>
<td>value</td>
<td>int</span></td>
<td>returns the current element associated value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-change="onChange"></div>
    <script>
        function onChange(args) {
            //handle the event
        }
    </script> 

{% endhighlight %}


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({
            change: function (args) {
                //handle the event
            }
        });
    </script>

{% endhighlight %}




### tap
{:#events:tap}




Event triggers when touch happens on the control.

<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>argument</td>
<td>Object</span></td>
<td>Event parameters from Rating.
<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>cancel</td>
<td>boolean</span></td>
<td>returns true if the event should be cancelled; otherwise, false.</td>
</tr>
<tr>
<td>type</td>
<td>string</span></td>
<td>returns the name of the event.</td>
</tr>
<tr>
<td>model</td>
<td>Object</span></td>
<td>returns the model value of the control.</td>
</tr>
<tr>
<td>value</td>
<td>int</span></td>
<td>returns the current element associated value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-tap="ontap"></div>
    <script>
        function ontap(args) {
            //handle the event
        }
    </script> 

{% endhighlight %}


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({
            tap: function (args) {
                //handle the event
            }
        });
    </script>

{% endhighlight %}


### touchMove
{:#events:touchmove}




Event triggers when touch move happens on the control.

<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>argument</td>
<td>Object</span></td>
<td>Event parameters from Rating.
<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>cancel</td>
<td>boolean</span></td>
<td>returns true if the event should be cancelled; otherwise, false.</td>
</tr>
<tr>
<td>type</td>
<td>string</span></td>
<td>returns the name of the event.</td>
</tr>
<tr>
<td>model</td>
<td>Object</span></td>
<td>returns the model value of the control.</td>
</tr>
<tr>
<td>value</td>
<td>int</span></td>
<td>returns the current element associated value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating" data-role="ejmrating" data-ej-touchmove="ontouchmove"></div>
    <script>
        function ontouchmove(args) {
            //handle the event
        }
    </script> 

{% endhighlight %}


{% highlight html %} 

    <!-- Unobtrusive way of rendering -->
    <div id="rating"></div>
    <script>
        $("#rating").ejmRating({
            touchmove: function (args) {
                //handle the event
            }
        });
    </script>

{% endhighlight %}



