---
layout: post
title: Image-Configuration | Tile | Mobilejs | Syncfusion
description: image configuration
platform: js
control: Tile (Mobile)
documentation: ug
keywords: tile, image
---

# Image configuration

The `data-ej-imageposition` attribute is used to adjust the position of the Tile image. It accepts the following values.

1. center

2. topcenter

3. bottomcenter

4. rightcenter

5. leftcenter

6. topleft

7. topright

8. bottomright

9. bottomleft

10. fill

The `data-ej-backgroundcolor` attribute is used to set the background color of the Tile.

The `data-ej-imageurl` attribute is used to specify the file name for the background image of the Tile. The `data-ej-imagepath` attribute is used to define the root path that should contain the following folder structure to automatically render the background image based on the device/platform it gets rendered. All these three folder should contain the image files (with same name, but different images) that can be specified in the image url property.

* **iOS7** - Folder name for ios7 specific images

* **Android** - Folder name for Android specific images

* **Windows** - Folder name for Windows specific images

N> Both `data-ej-imagepath` and `data-ej-imageurl` attribute can be set when you want to specify separate images for each render mode and so it is necessary to specify separate path for iOS, android and windows renderMode. When `data-ej-imageurl` attribute is alone used, you can provide common images for all render modes. So, you should provide the whole image path for this attribute.



{% highlight html %}

<div id="header" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>

<div class="tiles" style="top: 45px; position: relative;">
        <div id="tileview1" data-role="ejmtile" data-ej-showroundedcorner="true" data-ej-imageposition="fill" data-ej-caption-position="outer" data-ej-caption-alignment="center" data-ej-tilesize="small" data-ej-imagepath="../themes/sampleimages/tileview/" data-ej-caption-text="Settings" data-ej-imageurl="setting.png">
        </div>
    </div>    


{% endhighlight %}



The following screenshot displays the output of the above code.

![imagepath](image-configuration_images\image-configuration_img1.png)

Also you can give images for each Tile through **CSS** classes by using the `data-ej-imageclass` attribute. You can define your desired styles in the specified class.

Refer to the following code example.

{% highlight html %}


<div id=" header " data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>

<div class="tiles" style="top: 45px; position: relative;">
        <div id="tileview1" data-role="ejmtile" data-ej-showroundedcorner="true" data-ej-imageposition="fill" data-ej-imageclass="imageclass" data-ej-caption-position="outer" data-ej-caption-alignment="center" data-ej-tilesize="small" data-ej-caption-text="Settings">
        </div>
    </div>    



{% endhighlight %}

Refer the below code snippets for CSS classes

{% highlight css %}

     .imageclass {
            background-image: url("../themes/sampleimages/tileview/ios7/setting.png");
        }


{% endhighlight %}



The following screenshot illustrates the output of the above code.

![](image-configuration_images\image-configuration_img2.png)

