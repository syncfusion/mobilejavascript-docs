---
layout: post
title: ejmTile | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmTile
platform: Mobilejs
control: ejmTile
documentation: API
keywords: ejmTile, API, Essential Studio JS Tile (Mobile) 
---

# ejmTile


The Essential JavaScript Mobile Tile widget is a simple, opaque display of colored rectangles or squares that are arranged on the start screen in a grid-like pattern and it can be either static or live.

Custom Design for HTML Tile control.

$(element).ejmTile()



#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({ imageUrl: "themes/sample/tile/people.png" });
    </script>


{% endhighlight %}



#### Requires

* module:jQuery

* module:ej.mobile.application

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

* module:ej.tilebase

## Members

### allowSelection `Boolean`
{:#members:allowselection}

Specifies to allow the selection checkmark for Tile.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-allowselection="true">
    </div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            allowSelection: true,
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### backgroundColor `String`
{:#members:backgroundcolor}

Changes the background color of Tile.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="red">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            backgroundColor: "red"
        });
    </script>


{% endhighlight %}



### badge `Object`
{:#members:badge}

Section for badge specific functionalities.

### badge.enabled `Boolean`
{:#members:badge-enabled}

Specifies whether to enable badge or not.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-badge-enabled="true">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            badge: { enabled: true },
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### badge.maxValue `Number`
{:#members:badge-maxvalue}

Specifies maximum value for tile badge.

#### Default Value:

* 100

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-badge-enabled="true" data-ej-badge-value="5" data-ej-badge-maxvalue="3">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            badge: { enabled: true, value: 5, maxValue: 3 },
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### badge.minValue `Number`
{:#members:badge-minvalue}

Specifies minimum value for tile badge.

#### Default Value:

* 1

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-badge-enabled="true" data-ej-badge-value="3" data-ej-badge-minvalue="5" data-ej-backgroundcolor="red">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            badge: { enabled: true, value: 3, minValue: 5 },
            backgroundColor: "red"
        });
    </script>


{% endhighlight %}



### badge.position `Enum`
{:#members:badge-position}

Sets the tile badge position.

#### Default Value:

* “bottomright”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-badge-position="topright" data-ej-badge-enabled="true" data-ej-badge-value="5" data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            badge: { enabled: true, value: 5, position: "topright" },
            backgroundColor: "red"
        });
    </script>


{% endhighlight %}



### badge.text `String`
{:#members:badge-text}

Specifies text instead of number for tile badge.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-badge-enabled="true" data-ej-badge-text="ten" data-ej-backgroundcolor="red">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            badge: { enabled: true, text: "ten" },
            backgroundColor: "red"
        });
    </script>


{% endhighlight %}



### badge.value `Number`
{:#members:badge-value}

Sets value for tile badge.

#### Default Value:

* 1

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-badge-enabled="true" data-ej-badge-value="5" data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            badge: { enabled: true, value: 5 },
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### caption `Object`
{:#members:caption}

Section for live tile specific functionalities.

### caption.alignment `String`
{:#members:caption-alignment}

Specifies the caption alignment. See CaptionAlignment

#### Default Value:

* “normal”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-caption-alignment="left" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-tilesize="medium">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            backgroundColor: "blue",
            tileSize: "medium",
            caption: {
                alignment: "left"
            }
        });
    </script>


{% endhighlight %}



### caption.enabled `Boolean`
{:#members:caption-enabled}

Specifies whether to enable caption or not.

#### Default Value:

* true


#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-caption-enabled="false" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-tilesize="medium">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            backgroundColor: "blue",
            tileSize: "medium",
            caption: {
                enabled: false
            }
        });
    </script>


{% endhighlight %}



### caption.icon `String`
{:#members:caption-icon}

Specifies the caption icon.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-caption-icon="settings" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-tilesize="medium">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            backgroundColor: "blue",
            tileSize: "medium",
            caption: {
                icon: "settings"
            }
        });
    </script>


{% endhighlight %}



### caption.position `Enum`
{:#members:caption-position}

Specifies the caption position. See CaptionPosition

#### Default Value:

* “innerbottom”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-caption-position="outer" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-tilesize="medium">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            backgroundColor: "blue",
            tileSize: "medium",
            caption: {
                position: "outer"
            }
        });
    </script>


{% endhighlight %}



### caption.text `String`
{:#members:caption-text}

Specifies whether to enable caption or not.

#### Default Value:

* “text”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-caption-text="People" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-tilesize="medium">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
  <div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            backgroundColor: "blue",
            tileSize: "medium",
            caption: {
                text: "People"
            }
        });
    </script>


{% endhighlight %}



### cssClass `String`
{:#members:cssclass}

Sets the root class for Tile theme. This cssClass API helps to use custom skinning option for Tile control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* ””

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-cssclass="customclass">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            cssClass: "customclass",
        });
    </script>


{% endhighlight %}


### enablePersistence `Boolean`
{:#members:enablepersistence}

Saves current model value to browser cookies for state maintains. While refreshing the page retains the model value applies from browser cookies.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-enablepersistence="true">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            enablePersistence: true
        });
    </script>


{% endhighlight %}



### height `Number`
{:#members:height}

Customize the tile size height.

#### Default Value:

* “null”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-height=300 data-ej-width=300 data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({ imageUrl: "themes/sample/tile/people.png", width: 300, height: 300, backgroundColor: "blue" });
    </script>


{% endhighlight %}



### imageClass `String`
{:#members:imageclass}

Specifies Tile imageclass, using this property we can give images for each tile through css classes.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageclass="sample">
    </div>
    <style>
        .sample {
            background-image: url("themes/sample/tile/people.png");
        }
    </style>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({ imageClass: "sample" });
    </script>
    <style>
        .sample {
            background-image: url("themes/sample/tile/people.png");
        }
    </style>


{% endhighlight %}



### imagePath `String`
{:#members:imagepath}

Specifies the file path of tile image.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imagepath="themes/sample/tile" data-ej-imageurl="people.png">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imagePath: "themes/sample/tile",
            imageUrl: "people.png"
        });
    </script>


{% endhighlight %}



### imagePosition `Enum`
{:#members:imageposition}

Specifies the position of tile image.

#### Default Value:

* “center”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-imageposition="right" data-ej-backgroundcolor="red">
    </div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
  <div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            imagePosition: "right",
            backgroundColor: "red"
        });
    </script>


{% endhighlight %}



### imageTemplateId `String`
{:#members:imagetemplateid}

Specifies the tile image in outside template content.

#### Default Value:

* null

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imagetemplateid="sample">
    </div>
    <div id="sample" style="background-image: url('themes/sample/tile/ios7/people.png');height:100%;width:100%;">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <div id="sample" style="background-image: url('themes/sample/tile/ios7/people.png');height:100%;width:100%;">
    </div>
    <script>
        // Create Tile control
        $(function () {
            $("#tile").ejmTile({ imageTemplateId: "sample" });
        });
    </script>


{% endhighlight %}



### imageUrl `String`
{:#members:imageurl}

Specifies the file name of tile image.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({ imageUrl: "themes/sample/tile/people.png" });
    </script>


{% endhighlight %}



### liveTile `Object`
{:#members:livetile}

Section for live tile specific functionalities.


### liveTile.enabled `Boolean`
{:#members:livetile-enabled}

Specifies whether to enable live tile or not.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-rendermode="windows" data-ej-imagepath="themes/sample/tile" data-ej-livetile-imageurl="['people.png','sports.png']" data-ej-livetile-enabled="true" data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            renderMode: "windows",
            liveTile: {
                enabled: true,
                imageUrl: ['people.png', 'sports.png']
            },
            imagePath: "themes/sample/tile",
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### liveTile.imageClass `String`
{:#members:livetile-imageclass}

Specifies the live tile images in CSS classes.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-rendermode="windows" data-ej-livetile-imageclass="['img1','img2']" data-ej-livetile-enabled="true" data-ej-backgroundcolor="blue">
    </div>
    <style>
        .img1 {
            background-image: url("themes/sample/tile/windows/people.png");
        }

        .img2 {
            background-image: url("themes/sample/tile/windows/sports.png");
        }
    </style>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            renderMode: "windows",
            liveTile: {
                enabled: true,
                imageClass: ['img1', 'img2']
            },
            backgroundColor: "blue"
        });
    </script>
    <style>
        .img1 {
            background-image: url("themes/sample/tile/windows/people.png");
        }

        .img2 {
            background-image: url("themes/sample/tile/windows/sports.png");
        }
    </style>


{% endhighlight %}



### liveTile.imageTemplateId `String`
{:#members:livetile-imagetemplateid}

Specifies live Tile images in templates.

#### Default Value:

* null

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
  <div id="tile" data-role="ejmtile" data-ej-rendermode="windows" data-ej-livetile-imagetemplateid="['img1','img2','img3']" data-ej-livetile-enabled="true" data-ej-backgroundcolor="blue">
    </div>
    <div id="img1" style="background-image: url('themes/sample/tile/windows/people.png');height:100%;width:100%;">
    </div>
    <div id="img2" style="background-image: url('themes/sample/tile/windows/sports.png');height:100%;width:100%;">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <div id="img1" style="background-image: url('themes/sample/tile/windows/people.png');height:100%;width:100%;">
    </div>
    <div id="img2" style="background-image: url('themes/sample/tile/windows/sports.png');height:100%;width:100%;">
    </div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            renderMode: "windows",
            liveTile: {
                enabled: true,
                imageTemplateId: ['img1', 'img2']
            },
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}


### liveTile.imageUrl `String`
{:#members:livetile-imageurl}

Specifies the live tile image URL.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-rendermode="windows" data-ej-imagepath="themes/sample/tile" data-ej-livetile-imageurl="['people.png','sports.png']" data-ej-livetile-enabled="true" data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            renderMode: "windows",
            liveTile: {
                enabled: true,
                imageUrl: ['people.png', 'sports.png']
            },
            imagePath: "themes/sample/tile",
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### liveTile.text `String`
{:#members:livetile-text}

Specifies whether the live tile text.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-livetile-text=['People','Sports'] data-ej-rendermode="windows" data-ej-imagepath="themes/sample/tile" data-ej-livetile-imageurl="['people.png','sports.png']" data-ej-livetile-enabled="true" data-ej-backgroundcolor="red" data-ej-tilesize="medium">
    </div>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            renderMode: "windows",
            liveTile: {
                enabled: true,
                imageUrl: ['people.png', 'sports.png'],
                text: ['People', 'Sports']
            },
            imagePath: "themes/sample/tile",
            backgroundColor: "red",
            tileSize: "medium"
        });
    </script>


{% endhighlight %}



### liveTile.type `Enum`
{:#members:livetile-type}

Specifies the live tile type. See liveTile.type

#### Default Value:

* “flip”

#### Example

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <div id="tile" data-role="ejmtile" data-ej-rendermode="windows" data-ej-livetile-type="carousel" data-ej-imagepath="themes/sample/tile" data-ej-livetile-imageurl="['people.png','sports.png']" data-ej-livetile-enabled="true" data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            renderMode: "windows",
            liveTile: {
                enabled: true,
                imageUrl: ['people.png', 'sports.png'],
                type: "carousel"
            },
            imagePath: "themes/sample/tile",
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### liveTile.updateInterval `Int`
{:#members:livetile-updateinterval}

Specifies time interval between two successive live tile animation.

#### Default Value:

* 2000

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-rendermode="windows" data-ej-livetile-updateinterval="500" data-ej-imagepath="themes/sample/tile" data-ej-livetile-imageurl="['people.png','sports.png']" data-ej-livetile-enabled="true" data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
  <div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            renderMode: "windows",
            liveTile: {
                enabled: true,
                imageUrl: ['people.png', 'sports.png'],
                updateInterval: 500
            },
            imagePath: "themes/sample/tile",
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### renderMode `Enum`
{:#members:rendermode}

Changes the rendering mode of Tile. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value:

* auto

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-rendermode="android">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            renderMode: "android"
        });
    </script>


{% endhighlight %}



### showRoundedCorner `Boolean`
{:#members:showroundedcorner}

Specifies to show the rounded corner for tile.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-backgroundcolor="blue" data-ej-showroundedcorner="true">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            showRoundedCorner: true,
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### tileSize `Enum`
{:#members:tilesize}

Specifies the size of a tile. i.e small, medium, large or wide.

#### Default Value:

* “small”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-tilesize="large" data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering -->
   <div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            tileSize: "large",
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



### width `Number`
{:#members:width}

Customize the tile size width.

#### Default Value:

* “null”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-height=300 data-ej-width=300 data-ej-backgroundcolor="blue">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            width: 300,
            height: 300,
            backgroundColor: "blue"
        });
    </script>


{% endhighlight %}



## Methods

### updateTemplate()
{:#methods:updatetemplate}

Update the image template to another one.

#### Example

{% highlight html %}

<div id="tile" data-role="ejmtile" data-ej-imagetemplateid="sample1">
    </div>
    <div id="sample1" style="background-image: url('themes/sample/tile/ios7/people.png');height:100%;width:100%;">
    </div>
    <div id="sample2" style="background-image: url('themes/sample/tile/ios7/sports.png');height:100%;width:100%;">
    </div>
    <script>
        $(function () {
            var value = $("#tile").data("ejmTile");
            value.updateTemplate("sample2");
        });
    </script>


{% endhighlight %}



## Events

### touchEnd
{:#events:touchend}

Event triggers when the touchend happens in the tile

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
Event parameters from tile<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
boolean</td><td>
Returns the tile model</td></tr>
<tr>
<td>
type</td><td>
boolean</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
text</td><td>
boolean</td><td>
Returns the current tile text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-touchend="touchend">
    </div>
    <script>
        // touchEnd event for tile
        function touchend(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            touchEnd: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}



### touchStart
{:#events:touchstart}

Event triggers when the touchstart happens in the tile

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
Event parameters from tile<table><br><tr><br><th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
boolean</td><td>
Returns the tile model</td></tr>
<tr>
<td>
type</td><td>
boolean</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
text</td><td>
boolean</td><td>
Returns the current tile text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div id="tile" data-role="ejmtile" data-ej-imageurl="themes/sample/tile/people.png" data-ej-touchstart="touchstart">
    </div>
    <script>
        // touchStart event for tile
        function touchstart(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div id="tile"></div>
    <script>
        // Create Tile control
        $("#tile").ejmTile({
            imageUrl: "themes/sample/tile/people.png",
            touchStart: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}




