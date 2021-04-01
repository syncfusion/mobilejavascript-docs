---
layout: post
title: Mouse wheel scrolling | Scroll Panel | Mobilejs | Syncfusion
description: mouse wheel scrolling
platform: Mobilejs
control: Scroll Panel (Mobile)
documentation: ug
keywords : mouse , scroll
---

# Mouse wheel scrolling

The “data-ej-enablemousewheel” is a boolean attribute is used to decide whether  the ScrollPanel can be controlled by using mouse wheel or not. By default, this property is set to true.

You can adjust the scrolling speed with respect to Mouse wheel speed. This can be achieved by using “data-ej-wheelspeed” attribute. By default, this property is set to 16.

{% highlight html %}

<div data-role="ejmheader" data-ej-title="ScrollPanel"></div>

    <div id="maincontent" style="padding:10px">

        <div>

                       London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
            paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.

        </div>

    </div

<div id="sample_scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablemousewheel="true"  data-ej-enablenativescrolling="false"/>	

{% endhighlight %}