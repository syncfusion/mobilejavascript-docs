---
layout: post
title: ejmRotator | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmRotator
platform: Mobilejs
control: ejmRotator
documentation: API
keywords: ejmRotator, API, Essential Studio JS Rotator (Mobile) 
---

# ejmRotator

The Essential Mobile JavaScript Rotator control displays a set of slides. Each slide may contain images or images with content, or content with user-defined transition between them.

Custom Design for Html Rotator control.

$(element).ejmRotator();

####Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
 
 <div id="rotatorcontent">
        <div data-ej-imageurl="bird.jpg">
        </div>
        <div data-ej-imageurl="wheat.jpg">
        </div>
        <div data-ej-imageurl="card.jpg">
        </div>
        <div data-ej-imageurl="rose.jpg">
        </div>
        <div data-ej-imageurl="snowfall.jpg">
        </div>
        <div data-ej-imageurl="bird.jpg">
        </div>
    </div>
    <div id="rotator" data-role="ejmrotator" data-ej-targetid="rotatorcontent">
    </div>
	{% endhighlight %}
	
	{% highlight html %}
	
    <!-- Obtrusive way of rendering -->
     <div id="rotatorcontent">
        <div data-ej-imageurl="bird.jpg">
        </div>
        <div data-ej-imageurl="wheat.jpg">
        </div>
        <div data-ej-imageurl="card.jpg">
        </div>
        <div data-ej-imageurl="rose.jpg">
        </div>
        <div data-ej-imageurl="snowfall.jpg">
        </div>
        <div data-ej-imageurl="bird.jpg">
        </div>
    </div>
    <div id="rotator">
    </div>
    <script>
        $(function(){
            $("#rotator").ejmRotator({ targetId: "rotatorcontent" });
        })
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

### currentItemIndex `Int`
{:#members:currentitemindex}

Specifies the currentItemIndex for select the particular item based on the specified index.

#### Default Value:

* 0

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->

 <div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-currentitemindex="2">

    </div>

{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->

<div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotator">

    </div>

    <script>

        $(function () {

                       //To set currentItemIndex API value

            $("#rotator").ejmRotator({ targetId: "rotatorcontent", currentItemIndex: 2 });

        })

    </script>

{% endhighlight %}

### dataSource
{:#members:datasource}

Specifies the data source for Rotator rendering. In Rotator , options can be given as data source of JSON array.

#### Default Value:

* null

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<style>
    .image-bird
    {
        background-image: url("bird.jpg");
    }
        
    .image-wheat
    {
        background-image: url("wheat.jpg");
    }
        
    .image-card
    {
        background-image: url("card.jpg");
    }
        
    .image-rose
    {
        background-image: url("rose.jpg");
    }
        
    .image-snowfall
    {
        background-image: url("snowfall.jpg");
    }
</style>
<script type="text/javascript">

    window.dataSource = [{ imageUrl: 'image-bird' }, { imageUrl: 'image-wheat' }, { imageUrl: 'image-card' }, { imageUrl: 'image-rose' }, { imageUrl: 'image-snowfall'}];

</script>
<div id="rotatorcontent">
    <div class="e-m-rotator-image {{:imageUrl}}">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent"
    data-ej-datasource="window.dataSource">
</div>


{% endhighlight %}


{% highlight html %}

<style>
    .image-bird
    {
        background-image: url("bird.jpg");
    }
        
    .image-wheat
    {
        background-image: url("wheat.jpg");
    }
        
    .image-card
    {
        background-image: url("card.jpg");
    }
        
    .image-rose
    {
        background-image: url("rose.jpg");
    }
        
    .image-snowfall
    {
        background-image: url("snowfall.jpg");
    }
</style>
<div id="rotatorcontent">
    <div class="e-m-rotator-image {{:imageUrl}}">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set dataSource API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", dataSource: [{ imageUrl: 'image-bird' }, { imageUrl: 'image-wheat' }, { imageUrl: 'image-card' }, { imageUrl: 'image-rose' }, { imageUrl: 'image-snowfall'}] });

    })

</script>
	

{% endhighlight %}

### cssClass `String`
{:#members:cssclass}

Specify the CSS class to Rotator to achieve custom theme.

#### Default Value:

*“ ”

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<style>
    .customize-rotator .e-m-rotator-image
    {
        background-size: 200px 200px;
    }
</style>
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-cssclass="customize-rotator">
</div>


{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<style>
    .customize-rotator .e-m-rotator-image
    {
        background-size: 200px 200px;
    }
</style>
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set cssClass API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", cssClass: "customize-rotator" });

    })

</script>


{% endhighlight %}

### enablePersistence `Boolean`
{:#members:enablepersistence}

Current model value to browser cookies for state maintains. While refresh the Rotator control page retains the model value apply from browser cookies.

#### Default Value:

* false

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent"
    data-ej-enablepersistence="true">
</div>


{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set enablePersistence API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", enablePersistence: true });

    })
</script>

{% endhighlight %}

### items `Array`
{:#members:items}

Specifies the Rotator items as an array of JSON objects.

#### Default Value:

* null

#### Example  

{% highlight html %}

    <!-- Unobtrusive way of rendering -->

    <div id="rotatordefault" data-role="ejmrotator"  data-ej-items="[{imageUrl:'bird.jpg'},{imageUrl:'wheat.jpg'},{imageUrl:'card.jpg'},{imageUrl:'rose.jpg'},{imageUrl:'snowfall.jpg'}]">

    </div>


{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->


<div id="rotator">

    </div>

    <script>

        $(function () {

                       //To set items API value

            $("#rotator").ejmRotator({ items: [{ imageUrl: 'bird.jpg' }, { imageUrl: 'wheat.jpg' }, { imageUrl: 'card.jpg' }, { imageUrl: 'rose.jpg' }, { imageUrl: 'snowfall.jpg' }] });

        })

    </script>

{% endhighlight %}

### orientation `Enum`
{:#members:orientation}

Specifies the rotator orientation to the horizontal or vertical. See below to know available orientation options. 

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
Horizontal</td><td>
To swipe the rotator content images in horizontal</td></tr>
<tr>
<td>
Vertical</td><td>
To swipe the rotator content images in vertical</td></tr>
</table>

#### Default Value:

* “horizontal”

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent"
    data-ej-orientation="vertical">
</div>

{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set orientation API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", orientation: "vertical" });

    })

</script>

{% endhighlight %}

### pagerPosition `Enum`
{:#members:pagerposition}

Specifies the pager position relevant to orientation. See the below to know available pagerPosition options.



<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
Top</td><td>
To display the pager position on top side.</td></tr>
<tr>
<td>
Bottom</td><td>
To display the pager position on bottom side.</td></tr>
<tr>
<td>
Left</td><td>
To display the pager position on left side.</td></tr>
<tr>
<td>
Right</td><td>
To display the pager position on right side.</td></tr>
</table>


#### Default Value:

* “bottom”

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    s
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent"
    data-ej-pagerposition="top">
</div>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set pagerPosition API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", pagerPosition: "top" });

    })

</script>

{% endhighlight %}

### showPager `Boolean`
{:#members:showpager}

Specifies whether to show the Pager on initialization.

#### Default Value:

* true

#### Example  


{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent"
    data-ej-showpager="false">
</div>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set showPager API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", showPager: false });

    })

</script>

	
{% endhighlight %}

### renderMode `Enum`
{:#members:rendermode}

Specifies the rendering mode of the Rotator control. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Default</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
Auto</td><td>
string</td><td>
auto</td><td>
Auto RenderMode</td></tr>
<tr>
<td>
IOS7</td><td>
string</td><td>
ios7</td><td>
IOS7 RenderMode</td></tr>
<tr>
<td>
Android</td><td>
string</td><td>
android</td><td>
Android RenderMode</td></tr>
<tr>
<td>
Windows</td><td>
string</td><td>
windows</td><td>
Windows RenderMode</td></tr>
</table>


#### Default Value:

* auto



#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent"
    data-ej-rendermode="android">
</div>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set renderMode API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", renderMode: "android" });

    })

</script>

{% endhighlight %}

### targetHeight `String`
{:#members:targetheight}

Specifies the targetHeight on initialization of the Rotator control.

#### Default Value:

* auto

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent"
    data-ej-targetheight="300px">
</div>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set targetHeight API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent", targetHeight: "300px" });

    })

</script>

{% endhighlight %}


### targetId `String`
{:#members:targetid}

Specifies the targetId to the content of the Rotator control.

#### Default Value:

* null

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent">
</div>

{% endhighlight %}

{% highlight html %}


<!-- Obtrusive way of rendering -->
<div id="rotatorcontent">
    <div data-ej-imageurl="bird.jpg">
    </div>
    <div data-ej-imageurl="wheat.jpg">
    </div>
    <div data-ej-imageurl="card.jpg">
    </div>
    <div data-ej-imageurl="rose.jpg">
    </div>
    <div data-ej-imageurl="snowfall.jpg">
    </div>
    <div data-ej-imageurl="bird.jpg">
    </div>
</div>
<div id="rotator">
</div>
<script>

    $(function () {

        //To set targetId API value

        $("#rotator").ejmRotator({ targetId: "rotatorcontent" });

    })

</script>

{% endhighlight %}


### targetWidth `String`
{:#members:targetwidth}


Specifies the targetWidth on initialization of the Rotator control.

#### Default Value:

* auto

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->   

 <div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>s

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-targetwidth="300px">

    </div>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->

<div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotator">

    </div>

    <script>

        $(function () {

                   //To set targetWidth API value

            $("#rotator").ejmRotator({ targetId: "rotatorcontent", targetWidth: "300px" });

        })

    </script>

{% endhighlight %}

## Methods



### renderDatasource()
{:#methods:renderdatasource}

To handle the rotator datasource.

#### Example  

{% highlight html %}

<div id="rotator" data-role="ejmrotator" data-ej-targetid="rotatorcontent">

    </div>

    <div id="rotatorcontent">

        <div class="background-image:{{:imageUrl}};height:350px;width:630px">

        </div>

    </div>

    //To set the dataSource API value

    <script>

        $(function () {

            var imgdata = [{ imageUrl: 'bird.jpg' }, { imageUrl: 'wheat.jpg' }, { imageUrl: 'card.jpg' }, { imageUrl: 'rose.jpg' }, { imageUrl: 'snowfall.jpg' }];

            // To get the instance of the rotator control



            var rotObj = $("#rotator").data("ejmRotator");

            rotObj.renderDatasource(imgdata); 

        });

    </script>

{% endhighlight %}

## Events

### change
{:#events:change}

Event triggers when the rotator changes from one slide to another slide

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
returns the Rotator model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
argument.targetElement</td><td>
string</td><td>
returns the targetElement of the rotator</td></tr>
<tr>
<td>
argument.value</td><td>
number</td><td>
returns the current slide index.</td></tr>
</table>




#### Example  

{% highlight html %}

<div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>s

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-change="change">

    </div>

    <script>

        function change(args) {

            //handle the event

        }

    </script>

{% endhighlight %}



### pagerSelect
{:#events:pagerselect}

Event triggers when the rotator’s pager clicked

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
returns the Rotator model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
argument.targetElement</td><td>
string</td><td>
returns the targetElement of the rotator</td></tr>
<tr>
<td>
argument.value</td><td>
number</td><td>
returns the current slide index.</td></tr>
</table>


#### Example  

{% highlight html %}

<div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>s

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-pagerselect="pagerSelect">

    </div>

    <script>

        function pagerSelect(args) {

            //handle the event

        }

    </script>

{% endhighlight %}



### swipeDown
{:#events:swipedown}

Event triggers when the swipeDown happens in the Rotator

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
returns the Rotator model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
argument.targetElement</td><td>
string</td><td>
returns the targetElement of the rotator</td></tr>
<tr>
<td>
argument.value</td><td>
number</td><td>
returns the current slide index.</td></tr>
</table>


#### Example  

{% highlight html %}

<div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>s

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-swipedown="swipeDown">

    </div>

    <script>

        function swipeDown(args) {

            //handle the event

        }

    </script>

{% endhighlight %}


### swipeLeft
{:#events:swipeleft}

Event triggers when the swipeLeft happens.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
Returns the Rotator model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
argument.targetElement</td><td>
string</td><td>
Returns the targetElement of the Rotator</td></tr>
<tr>
<td>
argument.value</td><td>
number</td><td>
Returns the current slide index.</td></tr>
</table>


#### Example  

{% highlight html %}

  <div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>s

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-swipeleft="swipeLeft">

    </div>

    <script>

    function swipeLeft(args) {

        //handle the event

    }

    </script>

{% endhighlight %}

### swipeRight
{:#events:swiperight}

Event triggers when the swipeRight happens in the Rotator

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
returns the Rotator model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
argument.targetElement</td><td>
string</td><td>
returns the targetElement of the rotator</td></tr>
<tr>
<td>
argument.value</td><td>
number</td><td>
returns the current slide index.</td></tr>
</table>


#### Example  

{% highlight html %}

  <div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>s

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-swiperight="swipeRight">

    </div>

    <script>

        function swipeRight(args) {

            //handle the event

        }

    </script>

{% endhighlight %}

### swipeUp
{:#events:swipeup}

Event triggers when the swipeUp happens in the Rotator

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument.cancel</td><td>
boolean</td><td>
returns the cancel option value</td></tr>
<tr>
<td>
argument.model</td><td>
object</td><td>
returns the Rotator model</td></tr>
<tr>
<td>
argument.type</td><td>
string</td><td>
returns the name of the event</td></tr>
<tr>
<td>
argument.targetElement</td><td>
string</td><td>
returns the targetElement of the rotator</td></tr>
<tr>
<td>
argument.value</td><td>
number</td><td>
returns the current slide index.</td></tr>
</table>


#### Example  

{% highlight html %}

<div id="rotatorcontent">

        <div data-ej-imageurl="bird.jpg">

        </div>

        <div data-ej-imageurl="wheat.jpg">

        </div>

        <div data-ej-imageurl="card.jpg">

        </div>

        <div data-ej-imageurl="rose.jpg">

        </div>

        <div data-ej-imageurl="snowfall.jpg">

        </div>s

        <div data-ej-imageurl="bird.jpg">

        </div>

    </div>

    <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-swipeup="swipeUp">

    </div>

    <script>

        function swipeUp(args) {

            //handle the event

        }

    </script>

{% endhighlight %}



