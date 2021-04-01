---
layout: post
title: getting-started
description: getting started
platform: js
control: RadialMenu
documentation: ug
keywords: radialmenu
---

# Getting Started

This section explains briefly on how to create a Radial Menu control in your mobile application.

![](getting-started_images\getting-started_img1.png)

## Create basic mobile layout

Create an HTML file and paste the following template for mobile layout.     

{% highlight html %}

<!doctype html>
<html lang="en">
<head>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <title>Radialmenu</title>
<link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet"/>
<script src="http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js"></script>
<script src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
<script src="http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js"></script>
<script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"></script>
</head>
<body>
    <div>
        <!--- Adds Header Element Here  --->
        <!--- Adds Page Content Here  --->
        <!--- Adds Radialmenu Element Here  --->
    </div>
</body>
</html>



{% endhighlight %}



You can create header element with the following code.

{% highlight html %}

  <div id="header" data-role="ejmnavigationbar" data-ej-title="RadialMenu" data-ej-isrelative="true">
    </div>


{% endhighlight %}



Create the page content as follows.

{% highlight html %}

<div style="padding: 66px 25px; text-align: justify">
        <p>
           Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it.                             The model consists of application data, business rules, logic, and functions. A view can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible, such as a bar chart for management and a tabular view for accountants.
        </p>
    </div>


{% endhighlight %}



## Add RadialMenu control

Create a div element and set its data-role attribute as ejmradialmenu as follows.

{% highlight html %}

<div id="defaultradialmenu" data-role="ejmradialmenu">
     <ul>
          <!--- Add Menu Items Here  --->
     </ul>
</div>  



{% endhighlight %}

You can specify the images for each menu using data-ej-imageurl attribute for the inner list elements as follows. 

{% highlight html %}

<div id="defaultradialmenu" data-role="ejmradialmenu">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>


{% endhighlight %}

Run the above code to render the following output.

![](getting-started_images\add-radial-menu-control_img1.png)



