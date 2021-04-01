---
layout: post
title: orientation
description: orientation
platform: js
control: Rotator (Mobile)
documentation: ug
---

## Orientation

The data-ej-orientation attribute is used to swipe the Rotator in horizontal and vertical direction. By default, value of orientation is horizontal.

The pager is provided to indicate the item that is currently selected from the available number of items. The data-ej-showpager attribute is used to show the pager. The data-ej-pagerposition attribute is used to specify the pager position according to orientation. The data-ej-pagerposition possible values are as follows.

For vertical orientation

* left

* right



For horizontal orientation

* top

* bottom



Refer to the following code example.



Refer to the following code example.

{% highlight html %}

<div id="rotatordefault" data-role="ejmrotator" data-ej-showpager="true" data-ej-orientation="vertical" data-ej-targetid="rotatorcontentdefault">
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

{% highlight css %}


        .photo { 
            background-position: center center;  
            background-repeat: no-repeat;
            height: 100%; 
            width: 100%;  
            background-size:contain;
        }   
        .photo1 {     
            background-image: url(http://js.syncfusion.com/UG/Mobile/Content/rotator/tablet.jpg);    
        }      
        .photo2 {    
        background-image: url(http://js.syncfusion.com/UG/Mobile/Content/rotator/rose.jpg);  
        }      
        .photo3 {      
        background-image: url(http://js.syncfusion.com/UG/Mobile/Content/rotator/green.jpg);        
        }        
        .photo4 { 
        background-image: url(http://js.syncfusion.com/UG/Mobile/Content/rotator/nature.jpg); 
        }
        .photo5 {
        background-image: url(http://js.syncfusion.com/UG/Mobile/Content/rotator/snowfall.jpg);        
        }

        {% endhighlight %}


![](orientation_images\orientation_img1.png)

