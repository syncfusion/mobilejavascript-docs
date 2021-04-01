---
layout: post
title: Livetile-Configuration | Tile | Mobilejs | Syncfusion
description: livetile configuration
platform: js
control: Tile (Mobile)
documentation: ug
keywords: tile, livetile
---

# LiveTile configuration

**Live Tiles** are used to display the current or up to date information like scores, stocks, weather, etc. This functionality is supported only in windows rendermode. 

You can enable live Tile by using the `data-ej-livetile-enabled` attribute set to true that is the sub property of live Tile property. The `data-ej-livetile-type` attribute allows you to specify the type of animation while updating the information in the Tile. There are three types of Tile animation supported; flip, slide and carousel.

The `data-ej-livetile-imageurl` attribute sets background image for the Live Tile. This property accepts array values. So, you can specify the image url’s for all the Tiles that are used in the single Live Tile. 

You can specify the time interval for each Tile update/animation by using the `data-ej-livetile-updateinterval` attribute. The Time interval is given in **milliseconds**. The default value is **2000**

Refer to the following code example.

{% highlight html %}

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>
    <div class="tiles" style="top: 45px; position: relative;">
        <div id="tile6" data-role="ejmtile" data-ej-backgroundcolor="#3086e5" data-ej-rendermode="windows" data-ej-tilesize="medium" data-ej-imageposition="fill" data-ej-livetile-updateinterval="2500" data-ej-livetile-enabled="true" data-ej-livetile-type="slide" data-ej-livetile-imageurl="['../themes/sampleimages/tileview/windows/people_1.png','../themes/sampleimages/tileview/windows/people_2.png','../themes/sampleimages/tileview/windows/people_3.png']" data-ej-text="People">
        </div>
    </div>


{% endhighlight %}



By using the `data-ej-livetile-imagetemplateid` attribute, you can specify the Live Tile images outside the Tile rendering. To achieve this, you can provide image content inside the element where the path is specified by using the `templateid`. You can update the `imageTemplateId` dynamically through the `updateTemplateID` public method.

{% highlight html %}

<div id="header" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>
    <div class="tiles" style="top: 45px; position: relative;">
        <div id="tile" data-role="ejmtile" data-ej-rendermode="windows" data-ej-tilesize="medium" data-ej-caption-text="People" data-ej-imageposition="fill" data-ej-livetile-imagetemplateid=["temp1","temp2"] data-ej-livetile-enabled="true">
        </div>

    </div>
    <div id="temp1" style="background-image:
            url('../themes/sampleimages/tileview/windows/people_1.png'); width: 100%; height: 100%;">
    </div>
    <div id="temp2" style="background-image:
            url('../themes/sampleimages/tileview/windows/people_3.png'); width: 100%; height: 100%;">
    </div>


{% endhighlight %}



You can specify the array of images for the Live Tile through **CSS** classes by using the `data-ej-livetile-imageclass` attribute and you can define the desired styles in the specified class.

{% highlight html %}

  <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>
    <div class="tiles" style="top: 45px; position: relative;">
        <div id="tile" data-role="ejmtile" data-ej-tilesize="medium" data-ej-caption-text="People" data-ej-rendermode="windows" data-ej-imageposition="fill" data-ej-livetile-imageclass=["people_1","people_2"] data-ej-livetile-enabled="true">
        </div>


    </div>


{% endhighlight %}

Refer the below code snippets for CSS class

{% highlight css %}

  .people_1 {
            background-image: url('../themes/sampleimages/tileview/windows/people_1.png');
        }
        .people_2 {
            background-image: url('../themes/sampleimages/tileview/windows/people_2.png');
        }    


{% endhighlight %}





You can specify the array of caption text for the Live Tile by using the `data-ej-livetile-text` attribute.

{% highlight html %}

<div id="header" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>
    <div class="tiles" style="top: 45px; position: relative;">
        <div id="tile6" data-role="ejmtile" data-ej-rendermode="windows" data-ej-livetile-text="['John','Smith','Johnson']" data-ej-tilesize="medium" data-ej-imageposition="fill" data-ej-livetile-updateinterval="2500" data-ej-livetile-enabled="true" data-ej-livetile-type="slide" data-ej-livetile-imageurl="['../themes/sampleimages/tileview/windows/people_1.png','../themes/sampleimages/tileview/windows/people_2.png','../themes/sampleimages/tileview/windows/people_3.png']">
        </div>
    </div>


{% endhighlight %}





