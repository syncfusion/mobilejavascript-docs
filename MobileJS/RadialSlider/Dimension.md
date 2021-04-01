---
layout: post
title: dimension
description: dimension
platform: js
control: RadialSlider
documentation: radialslider,dimension
---

## Dimension

### Stroke width

Radial Slider strokeWidth property specifies the width of the outline. Refer to the following code example.

{% highlight html %}

<div class="radialslider default control">
        <div style="text-align: center">
            <button id="targetButton" data-role="ejmbutton" data-ej-touchend="radialslideropen" data-ej-text="Click here for image zooming"></button>
        </div>
    </div>
    <div id="defaultradialslider" data-role="ejmradialslider" data-ej-strokewidth="15" data-ej-autoopen="false" data-ej-position="bottomcenter" data-ej-change="sliderchange" data-ej-slide="sliderchange" data-ej-radius="150" data-ej-ticks="[30,35,40,45,50,55,60,65]" data-ej-value="50"></div>
    <div id="imagezoom">
    </div>


{% endhighlight %}

![](dimension_images\stroke-width_img1.png)

