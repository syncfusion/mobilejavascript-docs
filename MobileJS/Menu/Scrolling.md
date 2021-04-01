---
layout: post
title: Scrolling | Menu | Mobilejs | Syncfusion
description: scrolling 	
platform: Mobilejs
control: Menu (Mobile)
documentation: ug
keywords: scrolling
---

# Scrolling 	

The data-ej-allowscrolling attribute defines whether to allow the scrolling behavior or not when the number of Menu items exceed the specified Menu height.The default value of allowscrolling  property  is true

{% highlight html %}

 <div style="text-align: center;">

	<input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />

</div>

<div id="menu_sample" data-role="ejmmenu" data-ej-target="menuitem" data-ej-height="200">

	<ul>

		<li data-ej-text="Get info"></li>

		<li data-ej-text="Show in folder"></li>

		<li data-ej-text="Delete"></li>

		<li data-ej-text="Get info"></li>

		<li data-ej-text="Show in folder"></li>

		<li data-ej-text="Delete"></li>

		<li data-ej-text="Get info"></li>

		<li data-ej-text="Show in folder"></li>

		<li data-ej-text="Delete"></li>

	</ul>

</div>

{% endhighlight %}

The following screenshot displays Scrolling:

![](Scrolling_images/Scrolling_img1.png)