---
layout: post
title: Templating | Menu | Mobilejs | Syncfusion
description: templating
platform: Mobilejs
control: Menu (Mobile)
documentation: ug
keywords: template
---

## Templating	

 You can customize the appearance of an individual Menu item or the whole Menu is rendered with a single template.

{% highlight html %}

<div style="text-align: center;">

	<input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />

</div>

<div id="menu_sample" data-role="ejmmenu" data-ej-target="menuitem">

	<div style="text-align:center;">

	   <div><img class="image" src="twitter.gif" /><span class="text">Twitter</span></div>

	   <div><img class="image" src="facebook.gif" /><span class="text">Facebook</span></div>

	</div>

</div>

{% endhighlight %}

The following screenshot displays the RenderTemplate of Menu.

![](Templating_images/Templating_img1.png)

## TemplateID

This attribute is used to define the Template ID for the Menu item. Template is defined outside and can be rendered by using its ID for Menu items. The template’s ID is set to the data-ej-templateid attribute for the Menu control so that the template renders along with the Menu. 

{% highlight html %}

<div style="text-align: center;">

    <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" /> 
	
</div>

 <div style="text-align: center;">
            <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
        </div>
        <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-templateid="menuTemplate"></div>
        <div id="menuTemplate">
            <ul>
                <li>Get info</li>
                <li>Show in folder</li>
                <li>Delete</li>
            </ul>
        </div>

{% endhighlight %}