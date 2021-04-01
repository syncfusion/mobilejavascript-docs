---
layout: post
title: Badge-Configuration | Tile | Mobilejs | Syncfusion
description: badge configuration
platform: js
control: Tile (Mobile)
documentation: ug
keywords: tile, badge
---

# Badge configuration

The `badge` property handles badge specific functionalities like **enable** or **disable** the badge and setting badge value for the Tile. The `data-ej-badge-text` property is used to set the text instead of number for Tile badge. The `data-ej-badge-maxvalue` and `data-ej-badge-minvalue` attribute are used to set the **maximum** and **minimum** badge value to a Tile respectively. The `data-ej-badge-position` attribute is used to set the badge in `topleft` and `bottomleft` of a Tile.

Refer to the following code example.

{% highlight html %}

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>
    <div class="tiles" style="top: 45px; position: relative;">
        <div id="tileview1" data-role="ejmtile" data-ej-showroundedcorner="true" data-ej-badge-enabled="true" data-ej-badge-minvalue="10" data-ej-badge-maxvalue="80" data-ej-badge-value="88" data-ej-imageposition="fill" data-ej-caption-position="outer" data-ej-caption-alignment="center" data-ej-caption-text="Messaging" data-ej-imageurl="../themes/sampleimages/tileview/ios7/messaging.png">
        </div>
    </div>


{% endhighlight %}

The following screenshot illustrates the output of the above code.

![](badge-configuration_images\badge-configuration_img1.png)

