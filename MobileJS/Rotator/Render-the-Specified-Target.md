---
layout: post
title: render-the-specified-target
description: render the specified target
platform: js
control: Rotator (Mobile)
documentation: ug
---

## Render the specified target

You can render the contents for the Rotator by specifying the particular target element. The target element should maintain the HTML structure as mentioned in the following code example.

The data-ej-targetid attribute is used to define the Id of the target element where you can specify the content to render in the control. The data-ej-targetheight and data-ej-targetwidth attributes are used to specify the Rotator height and width respectively on initialization. Refer the following code example.

{% highlight html %}


            <div id="page">


        </div>   
        <div id="rotatordefault" data-role="ejmrotator" data-ej-targetid="rotatorcontentdefault">
        </div>

    <div id="rotatorcontentdefault">
        <div>
            <div class="photo photo1">
            </div>
        </div>
        <div>
            <div class="photo photo2">
            </div>
        </div>
        <div>
            <div class="photo photo3">
            </div>
        </div>
        <div>
            <div class="photo photo4">
            </div>
        </div>
        <div>
            <div class="photo photo5">
            </div>
        </div>
    </div>



{% endhighlight %}

![](render-the-specified-target_images\render-the-specified-target_img1.png)

