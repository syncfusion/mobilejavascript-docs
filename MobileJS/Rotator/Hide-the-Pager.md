---
layout: post
title: hide-the-pager
description: hide the pager
platform: js
control: Rotator (Mobile)
documentation: ug
---

## Hide the pager

You can see in the above image, the pager is to indicate the item that is currently displayed. You don’t need to show the pager in our use case. To achieve this, make “data-ej-showpager” attribute value as false.



{% highlight html %}


<div id="rotator" data-role="ejmrotator" data-ej-targetid="rotatorcontent" data-ej-showpager="false">
</div>



{% endhighlight %}

![](hide-the-pager_images\hide-the-pager_img1.png)

