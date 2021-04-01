---
layout: post
title: Select Item | Tab | Mobilejs | Syncfusion
description: select item
platform: Mobilejs
control: Tab (Mobile)
documentation: ug
keywords: select
---

# Select item

Tab control takes a numeric value given in “data-ej-selecteditemindex” attribute and selects the corresponding item that matches the given index. Default value for selectedItemIndex property is set to 0. You can refer the following code example.

{% highlight html %}



<div data-role="ejmtab" id="tab" data-ej-rendermode="ios7" data-ej-selecteditemindex="1" >

	<ul>

		<li data-ej-href="#mymusic" data-ej-text='My Music' data-ej-ios7-imageclass="icn-Mymusic"></li>

		<li data-ej-href="#favorites" data-ej-text='Favorites' data-ej-ios7-imageclass="icn-Favorites"></li>

		<li data-ej-href="#updates" data-ej-text='Updates' data-ej-ios7-imageclass="icn-Updates"></li>

	</ul>

</div>

<!-- Tab first item -->

<div data-role="ejmlistview" data-ej-showheader="false" id="mymusic">

    <ul>

        <li data-ej-text="Not Afraid"></li>

        <li data-ej-text="Get Lucky"></li>

        <li data-ej-text="Roar"></li>

        <li data-ej-text="Till I Collapse"></li>

    </ul>

</div>

<!-- Tab second item -->

<div data-role="ejmlistview" data-ej-showheader="false" id="favorites">

    <ul>

        <li data-ej-text="Dark Horse"></li>

        <li data-ej-text="Roar"></li>

    </ul>

</div>

<!-- Tab third item -->

<div data-role="ejmlistview" data-ej-showheader="false" id="updates">

 <ul>

     <li data-ej-text="New songs available for download"></li>

     <li data-ej-text="1.2.1 update available"></li>

 </ul>

</div>

{% endhighlight %}

The following screenshot displays the Selected Items:

![](Select-Item_images/Select-Item_img1.png)