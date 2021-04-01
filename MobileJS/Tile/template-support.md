---
layout: post
title: Template-Support | Tile | Mobilejs | Syncfusion
description: template support
platform: js
control: Tile (Mobile)
documentation: ug
keywords: tile, template
---

# Template support

The `data-ej-imagetemplateid` attribute is used to customize the image of a Tile by providing the specific template id respectively. 

Refer to the following code example.

{% highlight html %}


  <div id="header" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Tile" data-ej-titlealignment="center" data-ej-position="top" data-ej-touchend="tileSelection">
    </div>
    <div class="tiles" style="top: 45px; position: relative;">
        <div id="tileview1" data-role="ejmtile" data-ej-backgroundcolor="#3086e5" data-ej-tilesize="wide" data-ej-caption-text="Windows Store" data-ej-imagetemplateid="imageTemplate">
        </div>
    </div>
    <div id="imageTemplate">
        <div id="appimage">
        </div>
        <div class="tileMargin">
            <span class="caption">Google Search</span><br />
            <span class="description">The world’s information</span><br />
            <span class="sub">Free</span>
        </div>

    </div> 


{% endhighlight %}



Refer the below code snippets for CSS classes

{% highlight css %}

  #appimage {
            background-image: url("../themes/sampleimages/rating/google.png");
            background-repeat: no-repeat;
            width: 70px;
            height: 70px;
            background-size: 100%;
            float: left;
        }

        #imageTemplate {
            margin-top: 35px;
            margin-left: 10px;
        }

        .tileMargin {
            padding-left: 77px;
            color: white;
        }


{% endhighlight %}



The following screenshot illustrates the output of the above code.

![](template-support_images\template-support_img1.png)

