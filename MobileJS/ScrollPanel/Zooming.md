---
layout: post
title: Zooming | Scroll Panel | Mobilejs | Syncfusion
description: zooming
platform: Mobilejs
control: Scroll Panel (Mobile)
documentation: ug
---

# Zooming

The “data-ej-enablezoom” is a boolean attribute that lets you specify whether the scrolling content can be zoomed or not. By default, this property is set to “false”.

{% highlight html %}

<div data-role="ejmheader" data-ej-title="ScrollPanel"></div>

<div id="maincontent" style="padding:10px">

	<div>

		Founded by industry experts in 2001, Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform. With Syncfusion, developers can move beyond simply coding applications to delivering real business innovation—the elegant user interfaces, business intelligence dashboards, and sophisticated reporting that today's business users need, in the formats they demand. Our award-winning .NET components and controls are designed to meet your evolving development needs, whether you're working in Windows Forms, WPF, ASP.NET, ASP.NET MVC, or Silverlight. At Syncfusion, we uncompromisingly strive for excellence in order to offer the very best value to our customers—from small ISVs to Fortune 100 companies. Our most successful product is Essential Studio.

	</div>

</div>

<div id="sample_scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablezoom="true" data-ej-startzoom="2" data-ej-enablenativescrolling="false" /> 

{% endhighlight %}

The following screenshot displays zooming:

![](Zooming_images/Zooming_img1.png)

## Zooming max

The “data-ej-zoommax” attribute lets you set the maximum limit to which the content can be zoomed. By default, this property is set to 6.

{% highlight html %}

<div data-role="ejmheader" data-ej-title="ScrollPanel"></div>

<div id="maincontent" style="padding:10px">

	<div>

		Founded by industry experts in 2001, Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform. With Syncfusion, developers can move beyond simply coding applications to delivering real business innovation—the elegant user interfaces, business intelligence dashboards, and sophisticated reporting that today's business users need, in the formats they demand. Our award-winning .NET components and controls are designed to meet your evolving development needs, whether you're working in Windows Forms, WPF, ASP.NET, ASP.NET MVC, or Silverlight. At Syncfusion, we uncompromisingly strive for excellence in order to offer the very best value to our customers—from small ISVs to Fortune 100 companies. Our most successful product is Essential Studio.

	</div>

</div>

<div id="sample_scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablenativescrolling="false" data-ej-startzoom="2" data-ej-enablezoom="true" data-ej-zoommax="1" />

{% endhighlight %}

## Zooming  min

The “data-ej-zoommin” attribute lets you set the minimum limit to which the content can be zoomed. By default, this property is set to 1.

{% highlight html %}

<div data-role="ejmheader" data-ej-title="ScrollPanel"></div>

<div id="maincontent" style="padding:10px">

	<div>

		Founded by industry experts in 2001, Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform. With Syncfusion, developers can move beyond simply coding applications to delivering real business innovation—the elegant user interfaces, business intelligence dashboards, and sophisticated reporting that today's business users need, in the formats they demand. Our award-winning .NET components and controls are designed to meet your evolving development needs, whether you're working in Windows Forms, WPF, ASP.NET, ASP.NET MVC, or Silverlight. At Syncfusion, we uncompromisingly strive for excellence in order to offer the very best value to our customers—from small ISVs to Fortune 100 companies. Our most successful product is Essential Studio.

	</div>

</div>

<div id="sample_scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-startzoom="1" data-ej-enablezoom="true" data-ej-enablenativescrolling="false" data-ej-zoommin="2" />

{% endhighlight %}

## Start zooming

The “data-ej-startzoom” attribute lets you specify the zooming value on initial rendering of the scrollable content.  By default this property is set to 1.

{% highlight html %}

<div data-role="ejmheader" data-ej-title="ScrollPanel"></div>

<div id="maincontent" style="padding:10px">

	<div>

		Founded by industry experts in 2001, Syncfusion, Inc. provides the broadest range of enterprise-class software components and tools for the Microsoft .NET platform. With Syncfusion, developers can move beyond simply coding applications to delivering real business innovation—the elegant user interfaces, business intelligence dashboards, and sophisticated reporting that today's business users need, in the formats they demand. Our award-winning .NET components and controls are designed to meet your evolving development needs, whether you're working in Windows Forms, WPF, ASP.NET, ASP.NET MVC, or Silverlight. At Syncfusion, we uncompromisingly strive for excellence in order to offer the very best value to our customers—from small ISVs to Fortune 100 companies. Our most successful product is Essential Studio.

	</div>

</div>

<div id="sample_scrollpanel" data-role="ejmscrollpanel" data-ej-target="maincontent" data-ej-enablezoom="true" data-ej-startzoom="2" />

{% endhighlight %}

