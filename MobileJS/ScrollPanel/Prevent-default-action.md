---
layout: post
title: Prevent default action | Scroll Panel | Mobilejs | Syncfusion
description: prevent default action
platform: Mobilejs
control: Scroll Panel (Mobile)
documentation: ug
---

# Prevent default action

 While using ScrollPanel, you can prevent the default action by using “data-ej-preventdefault” attribute.  By default, this property is set to true.

{% highlight html %}

<div data-role="ejmheader" data-ej-title="ScrollPanel"></div>

    <div id="maincontent" style="padding:10px">

        <div>

                       London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
            paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.

        </div>

    </div>

<div id="sample_scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-preventdefault="true" data-ej-enablenativescrolling="false" />

{% endhighlight %}