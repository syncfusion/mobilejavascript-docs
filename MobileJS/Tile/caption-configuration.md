---
layout: post
title: Caption-Configuration | Tile | Mobilejs | Syncfusion
description: caption configuration
platform: js
control: Tile (Mobile)
documentation: ug
keywords: tile, caption
---

# Caption Configuration

The `data-ej-caption-enabled` attribute is used to show or hide the **Tile caption**. The `data-ej-caption-text` attribute is used to set the caption of a Tile. The `data-ej-caption-alignment` attribute is used to align the Tile text based on the requirement. The possible position values for `alignment` are as follows.

1. normal

2. left

3. right

4. center

The `data-ej-caption-position` attribute wraps the text inside or outside of a Tile. The possible position values of `data-ej-caption-position` are innertop, innerbottom and outer.

N> Caption position is not supported in small Tiles except ios and android outer position.



{% highlight html %}

  <div id="header" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>
    <div class="tiles" style="top: 45px; position: relative;">
        <div id="tileview1" data-role="ejmtile" data-ej-showroundedcorner="true" data-ej-imageposition="fill" data-ej-caption-position="outer" data-ej-caption-alignment="center" data-ej-tilesize="small" data-ej-caption-text="Weather" data-ej-imageurl="../themes/sampleimages/tileview/ios7/weather.png">
        </div>
    </div>


{% endhighlight %}



The following screenshot illustrates the output of the above code.

![](caption-configuration_images\caption-configuration_img1.png)

