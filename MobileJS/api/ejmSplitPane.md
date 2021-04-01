---
layout: post
title: ejmSplitPane | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmSplitPane
platform: Mobilejs
control: ejmSplitPane
documentation: API
keywords: ejmSplitPane, API, Essential Studio JS SplitPane (Mobile)
---

# ejmSplitPane

The Essential JavaScript Mobile SplitPane divides a region on the web page. It is configured to split up the horizontal view vertically. Center pane displays content from an external URL that is specific to the item selected in the left pane or right pane.

Custom Design for HTML SplitPane control.

$(element).ejmSplitPane()

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}




{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane();
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

### contentPane
{:#members:contentpane}

Specifies content pane specific properties.


### contentPane.templateId `string`
{:#members:contentpane-templateid}

Specifies Id for template content of content pane.

#### Default Value

* null



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-contentpane-templateid="contenttemplate">
        <div id="target2" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
    </div>

    <script id="contenttemplate" type="text/x-jsrender">
            <div>Main contents goes here</div>
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target2" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
    </div>

    <script id="contenttemplate" type="text/x-jsrender">
            <div>Main contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ contentPane: { templateId: "contenttemplate" } });
    </script>



{% endhighlight %}



### cssClass `string`
{:#members:cssclass}

Sets the root class for SplitPane theme. This cssClass API helps to use custom skinning option for SplitPane control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-cssclass="customclass">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <style>
        .customclass * {
            color: red;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ cssClass: "customclass" });
    </script>

    <style>
        .customclass * {
            color: red;
        }
    </style>



{% endhighlight %}



### edgeThreshold `number`
{:#members:edgethreshold}

Sets swipe threshold width for both left and right panes.

#### Default Value

* 50

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-edgethreshold="100">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ edgeThreshold: 100 });
    </script>



{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence}

Saves current model value to browser cookies for state maintains. While refreshing the page retains the model value apply from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-enablepersistence="true">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ enablePersistence: true });
    </script>



{% endhighlight %}



### enableSwipe `boolean`
{:#members:enableswipe}

Enable or Disable the swiping behavior to the content.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-enableswipe="false">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ enableSwipe: false });
    </script>



{% endhighlight %}



### height `string`
{:#members:height}

Specifies the height of the SplitPane. 

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-height="300px">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ height: "300px" });
    </script>



{% endhighlight %}



### isRelative `string`
{:#members:isrelative}

Sets relative position to the SplitPane if this property is true. Otherwise absolute position. 

N> If you set relative positioning for SplitPane, you should set height for SplitPane.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <br /><br /><br />
    <div id="splitview" data-role="ejmsplitpane" data-ej-isrelative="true" data-ej-height="200px">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <br /><br /><br />
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ isRelative: true, height: "200px" });
    </script>



{% endhighlight %}



### leftPane
{:#members:leftpane}

Specifies left pane specific properties.

### leftPane.animationType `enum`
{:#members:leftpane-animationtype}

Specifies the animation type for leftpane on its open or close. See SliptpaneAnimationType

N> To animate leftpane while opening or closing, set the property leftPane.showOnTablet to false.

#### Default Value

* “overlay”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-leftpane-showontablet="false" data-ej-leftpane-animationtype="reveal">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ leftPane: { showOnTablet: false, animationType: "reveal" } });
    </script>



{% endhighlight %}



### leftPane.showOnTablet `boolean`
{:#members:leftpane-showontablet}

Specifies the leftpane visibility for tablet devices. If this property set as false, the leftpane will be hidden and it will be open from left side window on swipe.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-leftpane-showontablet="false">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ leftPane: { showOnTablet: false } });
    </script>



{% endhighlight %}



### leftPane.templateId `string`
{:#members:leftpane-templateid}

Specifies Id for template content of leftpane.

#### Default Value

* null



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-leftpane-templateid="lefttemplate">
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="lefttemplate" type="text/x-jsrender">
            <div>Leftpane contents goes here</div>
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="lefttemplate" type="text/x-jsrender">
        <div>Leftpane contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ leftPane: { templateId: "lefttemplate" } });
    </script>



{% endhighlight %}



### leftPane.width `string`
{:#members:leftpane-width}

Specifies the width of leftpane.

#### Default Value

* “280px”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-leftpane-width="350px">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ leftPane: { width: "350px" } });
    </script>



{% endhighlight %}



### renderMode `enum`
{:#members:rendermode}

Changes the rendering mode of the SplitPane. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global.html#rendermode)

#### Default Value

* auto

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-rendermode="android">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ renderMode: "android" });
    </script>



{% endhighlight %}



### rightPane
{:#members:rightpane}

Specifies right pane specific properties.

### rightPane.animationType `enum`
{:#members:rightpane-animationtype}

Specifies the animation type for rightpane on its open or close. See SliptpaneAnimationType

N> To animate rightpane while opening or closing, set the property rightPane.showOnTablet to false.

#### Default Value

* “overlay”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-rightpane-showontablet="false" data-ej-rightpane-animationtype="reveal">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">

        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({rightPane: { showOnTablet: false, animationType: "reveal" } });
    </script>



{% endhighlight %}



### rightPane.showOnTablet `boolean`
{:#members:rightpane-showontablet}

Specifies the rightpane visibility for tablet devices. If this property set as false, the rightpane will be hidden and it will be open from right side window on swipe.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-rightpane-showontablet="true">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">

        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ rightPane: { showOnTablet: true } });
    </script>



{% endhighlight %}



### rightPane.templateId `string`
{:#members:rightpane-templateid}

Specifies Id for template content of rightpane.

#### Default Value

* null



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-rightpane-templateid="righttemplate">

        <div id="target2" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="righttemplate" type="text/x-jsrender">
            <div>Rightpane contents goes here</div>
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">

        <div id="target2" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="righttemplate" type="text/x-jsrender">
        <div>Rightpane contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ rightPane: { templateId: "righttemplate" } });
    </script>



{% endhighlight %}



### rightPane.width `string`
{:#members:rightpane-width}

Specifies the width of rightpane.

#### Default Value

* “280px”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-rightpane-width="350px">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">

        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ rightPane: { width: "350px" } });
    </script>



{% endhighlight %}



### stopEventPropagation `boolean`
{:#members:stopeventpropagation}

Stops event propagation for other elements. 

#### Default Value

* true if windows render mode, otherwise false.

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-stopeventpropagation="true">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ stopEventPropagation: true });
    </script>



{% endhighlight %}



### width `string`
{:#members:width}

Specifies the width of the SplitPane. 

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-width="700px">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        $("#splitview").ejmSplitPane({ width: "700px" });
    </script>



{% endhighlight %}



## Methods

### closePane()
{:#methods:closepane}

To close the currently opened pane.

#### Example

{% highlight html %}


    <div id="splitview" data-role="ejmsplitpane" data-ej-leftpane-animationtype="reveal"  data-ej-leftpane-showontablet="false">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <input data-role="ejmbutton" type="button" data-ej-text="Open LeftPane" data-ej-touchend="open" />
            <input data-role="ejmbutton" type="button" data-ej-text="Close Pane" data-ej-touchend="close" />
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function open() {
            $("#splitview").ejmSplitPane("openLeftPane");
        }
        function close() {
            $("#splitview").ejmSplitPane("closePane");
        }
    </script>



{% endhighlight %}



### openLeftPane()
{:#methods:openleftpane}

To open leftpane on demand.

#### Example

{% highlight html %}


    <div id="splitview" data-role="ejmsplitpane" data-ej-leftpane-showontablet="false">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <input data-role="ejmbutton" type="button" data-ej-text="Open LeftPane" data-ej-touchend="open" />
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function open() {
            $("#splitview").ejmSplitPane("openLeftPane");
        }
    </script>



{% endhighlight %}



### openRightPane()
{:#methods:openrightpane}

To open rightpane on demand.

#### Example

{% highlight html %}


    <div id="splitview" data-role="ejmsplitpane">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <input data-role="ejmbutton" type="button" data-ej-text="Open RightPane" data-ej-touchend="open" />
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function open() {
            $("#splitview").ejmSplitPane("openRightPane");
        }
    </script>



{% endhighlight %}



## Events

### beforeClose
{:#events:beforeclose}

Event triggers before the leftpane or rightpane closing.

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
Event parameters from SplitPane.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
panel</td><td>
string</td><td>
Returns the panel which is closing</td></tr>
<tr>
<td>
content</td><td>
object</td><td>
Returns closing panel contents as HTML elements</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns closing panel as HTML elements</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-beforeclose="close">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function close(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="lefttemplate" type="text/x-jsrender">
        <div>Leftpane contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ beforeClose: "close" });
        function close(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



### beforeOpen
{:#events:beforeopen}

Event triggers before the leftpane or rightpane opening.

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
Event parameters from SplitPane.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
panel</td><td>
string</td><td>
Returns the panel which is closing</td></tr>
<tr>
<td>
content</td><td>
object</td><td>
Returns opening panel contents as HTML elements</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns opening panel as HTML elements</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-beforeopen="open">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function open(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="lefttemplate" type="text/x-jsrender">
        <div>Leftpane contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ beforeopen: "open" });
        function open(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



### close
{:#events:close}

Event triggers while the leftpane or rightpane close.

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
Event parameters from SplitPane.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
panel</td><td>
string</td><td>
Returns the panel which is closing</td></tr>
<tr>
<td>
content</td><td>
object</td><td>
Returns closed panel contents as HTML elements</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns closed panel as HTML elements</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-close="close">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function close(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="lefttemplate" type="text/x-jsrender">
        <div>Leftpane contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ close: "close" });
        function close(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



### open
{:#events:open}

Event triggers while the leftpane or rightpane open.

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
Event parameters from SplitPane.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
panel</td><td>
string</td><td>
Returns the panel which is closing</td></tr>
<tr>
<td>
content</td><td>
object</td><td>
Returns opened panel contents as HTML elements</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns opened panel as HTML elements</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-open="open">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function open(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="lefttemplate" type="text/x-jsrender">
        <div>Leftpane contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ open: "open" });
        function open(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



### swipe
{:#events:swipe}

Event triggers while swipe happens in the page to open leftpane or rightpane.

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
Event parameters from SplitPane.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
event</td><td>
object</td><td>
Returns the event object which contains information about the event</td></tr>
<tr>
<td>
direction</td><td>
string</td><td>
Returns the direction from which swipe event happens</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="splitview" data-role="ejmsplitpane" data-ej-swipe="swipe">
        <div id="target1" data-ej-pane="left">
            <div>Leftpane contents goes here</div>
        </div>
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script>
        function swipe(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="splitview">
        <div id="target2" data-ej-pane="right">
            <div>Rightpane contents goes here</div>
        </div>
        <div id="target3" data-ej-pane="content">
            <div>Main contents goes here</div>
        </div>
    </div>

    <script id="lefttemplate" type="text/x-jsrender">
        <div>Leftpane contents goes here</div>
    </script>

    <script>
        $("#splitview").ejmSplitPane({ swipe: "swipe" });
        function swipe(args) {
            //Handle the event
        }
    </script>



{% endhighlight %}



