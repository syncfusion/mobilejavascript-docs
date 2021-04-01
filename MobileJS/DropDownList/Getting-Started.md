---
layout: post 
title: Getting started | DropDownList | Mobilejs | Syncfusion 
description: Getting starting 
platform: Mobilejs 
control: DropDownList (Mobile) 
documentation: ug
---

# Getting started

This section explains briefly about how to create a dropdownlist in your application with JavaScript.
Essential JavaScript dropdownlist provides support for multiple selections, within your web page and allows you to specify an option from the list. 
The following screenshot demonstrates the functionality with dropdownlist action.

![](getting-started-images/img1.png)

For getting started you can use the ‘ej.mobile.all.min.js’ file, which encapsulates all the ‘ejm’ controls and frameworks in one single file.
For themes, you can use the ‘ej.mobile.all.min.css’ CDN link from the snippet given. To add the themes in your application, please refer this link.

## Create basic mobile layout

Create an HTML file and paste the following template for mobile layout.

{% highlight html %}

<!DOCTYPE html>
<html>
<head>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <title>Navigation Drawer</title>
    <link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>                
    <script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"></script> 
</head>
<body>
    <div data-role="appview">
        <!-- Adding Header Control Here -->
        <!-- Adding DropDownlist Control here -->
		<!--Adding list of Options -->
    </div>
</body>
</html>

{% endhighlight %}

## Create DropDownList control

To Create DropDownList control, specify ejmdropdownlist as data-role attribute for a &#60;input&#62; element. You can set the text for list items by using data-ej-text attribute.

{% highlight html %}

    <!-- Adding DropDownList Control here -->
    <div class="sample-control default dropdownlist">
        <input type="text" id="dd_default" data-role="ejmdropdownlist" data-ej-watermarktext="Select search engine" />
    </div>
   
   <!--Adding list of Options -->
   
{% endhighlight %}

Run the above code to render the following output.

![](getting-started-images/img3.png)

## Add list of options

Specifies the data-ej-targetid attribute for  target element which consists the list of options to render DropDownList. 

{% highlight html %}

    <!-- Adding DropDownList Control here -->
  <div class="sample-control default dropdownlist">
        <input type="text" id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-watermarktext="Select search engine" />
    </div>
	<!--Adding list of options -->
    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo! Search"></li>
        <li data-ej-text="Ask"></li>
        <li data-ej-text="Aol Search"></li>
        <li data-ej-text="Wow"></li>
        <li data-ej-text="WebCrawler"></li>
        <li data-ej-text="MyWebSearch"></li>
        <li data-ej-text="Infospace"></li>
        <li data-ej-text="DuckDuckGo"></li>
        <li data-ej-text="Blekko"></li>
        <li data-ej-text="Contenko"></li>
    </ul>

{% endhighlight %}

Run the above code to render the following output.

![](getting-started-images/img1.png)

## Styles and appearance

Sets the root class for DropDownList. This cssClass API helps to use custom skinning option for DropDownList control. By defining the root class using this API, we need to include this root class in CSS.

{% highlight html %}

    <!-- Adding DropDownList Control here -->
  <div class="sample-control default dropdownlist">
        <input type="text" id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-watermarktext="Select search engine" data-ej-cssclass="custom class"    />
    </div>
    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo! Search"></li>
        <li data-ej-text="Ask"></li>
        <li data-ej-text="Aol Search"></li>
    
   <style>
        .customclass .e-m-dropdownlist {
            color: red !important;
        }
    </style>
    </ul>

{% endhighlight %}

Run the above code to render the following output.

![](getting-started-images/img2.png)




