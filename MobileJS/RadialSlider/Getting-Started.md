---
layout: post
title: getting-started
description: getting started
platform: js
control: RadialSlider
documentation: ug
keywords: radialslider
---

# Getting Started

This section explains briefly on how to create a Radial Slider control in your mobile application.

![](getting-started_images\getting-started_img1.png)

## Create basic mobile layout

Create an HTML file and paste the following template for mobile layout.     

{% highlight html %}

<!doctype html>
<html lang="en">
<head>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <title>RadialSlider</title>
<link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet"/>
<script src="http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js"></script>
<script src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
<script src="http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js"></script>
<script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"></script>
</head>
<body>
    <div>
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Radial Slider" data-ej-isrelative="true"></div>

        <!--- Adds RadialSlider Element Here  --->
    </div>
</body>
</html>



{% endhighlight %}

## Add Radial Slider control

Add the below code to render the Radial Slider

{% highlight html %}

 <div class="radialslider default control">
        <div style="text-align: center">
            <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialslideropen" data-ej-text="Click here for image zooming"></button>
        </div>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-autoopen="false" data-ej-position="bottomcenter" data-ej-change="sliderchange" data-ej-slide="sliderchange" data-ej-radius="150" data-ej-ticks="[30,35,40,45,50,55,60,65]" data-ej-value="50"></div>
    <div id="imagezoom">
    </div>


{% endhighlight %}



{% highlight js %}

function RadialSliderLoad() {
            if ($("#appList").is(":visible"))
                $("#defaultradialslider").css("left", parseInt($("#defaultradialslider").css("left")) - 140)
        }
        function radialslideropen(args) {

            $("#defaultradialslider").ejmRadialSlider("show");
        }
        function sliderchange(args) {
            $("#imagezoom").css("background-size", args.value + "%")
        }
        function RadialSliderRenderModeLoad() {
            $("#defaultradialslider").ejmRadialSlider({ value: 50, ticks: [30, 35, 40, 45, 50, 55, 60, 65] });
            $("#imagezoom").css("background-size", "50%")
        }


{% endhighlight %}

![](getting-started_images\add-radial-slider-control_img1.png)

