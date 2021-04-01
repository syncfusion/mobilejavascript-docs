---
layout: post
title: Getting Started | Progress Bar | Mobilejs | Syncfusion
description: getting started
platform: Mobilejs
control: Progress Bar (Mobile)
documentation: ug
keywords: progressbar, text, value
---

# Getting Started

The Essential JavaScript Mobile Progress Bar widget shows the progress of a lengthy operation by filling a rectangle with chunks from left to right.

In this section, you can learn how to create ProgressBar and how to use it in your application.

## Create your first ProgressBar in JavaScript

The Essential JavaScript Mobile Progress Bar is a simple interface to indicate the current progress of an operation, such as uploading a document. In the following guidelines, you will learn about the features in progress bar widget by creating an App Installer.

![](Getting-Started_images/Getting-Started_img1.png)

## Create the required layout for App Installer

Essential JavaScript Mobile progress bar widget can be rendered from a div element with corresponding properties. You can easily customize progress bar control by changing their properties according to your need. In our app installer, the progress bar is used to show the progress of installation. 

Create an HTML file and paste the following template to it for Progress Bar creation.

{% highlight html %}

<!DOCTYPE html>

<html>

	<head>
		<title>Progressbar</title>
        <link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
        <script src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>
        <script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"> </script>
    
	</head>

	<body>

        <div id="page" data-role="appview">

        <!-- header control -->

        <div data-role="ejmheader" data-ej-title="App Installer">

        </div>

        <div id="content">

        <div> 

        <!-- Add image and definition -->

        <div align="center">

        <img src="[http://js.syncfusion.com/UG/Mobile/Content/debug.png](http://js.syncfusion.com/UG/Mobile/Content/debug.png)" style="width: 125px;" /> </div> <br/><br />

        <div id="definition" align="center" style="padding: 0 20px">

        <b>BUG DETECTIVE</b><br />

                    Bug Detective is an open source application which integrates with web browsers to debug web development tools while you browse. We can debug HTML and JavaScript live in any web page using bug detective.

        </div><br/>

        <!-- Button control -->

        <div align="center">

        <input type="button" data-role="ejmbutton" data-ej-text="Install" id="button" data-ej-touchend="startProgress" /></div>

        <!--Add progressbar Element here-->

        </div></div> 

        <!-- ScrollPanel -->

 		<div data-role="ejmscrollpanel" data-ej-target="content"></div>

        </div>

	</body>

</html>

{% endhighlight %}

Run the above code to render the following output.

![](Getting-Started_images/Getting-Started_img2.png)


## Create ProgressBar control

To render the progress bar control, you need to set “data-role” attribute as “ejmprogress” to a div element.  Its initial value can be set using “data-ej-value” attribute. By default, it takes parent’s width. But you can customize by using “data-ej-width” attribute.

{% highlight html %}

<!--Progress bar control -->

<div style="width: 75%; margin:auto;" >

	<div id="progress" data-role="ejmprogress" data-ej-value="73">

	</div>

</div>

{% endhighlight %}

Progress bar can be hidden with a desired action on its “hide” API and can be shown with desired action on its “show” API. Refer the below code snippets.

{% highlight js %}

$(function () {

window.progressObject = $("#progress").data("ejmProgress"); // create object for progressbar

$("#progress").hide();//to hide progressbar at initialize

});

function startProgress(args) {

$(".e-m-btnwrapper").hide();//to hide button

$("#progress").show();// to show progressbar

}

{% endhighlight %}

Run this code and you will see the below output while clicking install button.

![](Getting-Started_images/Getting-Started_img3.png)

## Customize the text

The default text of progress bar is “downloading”. In our scenario we are installing the app, not downloading it. So to change the text of progress bar, we use “data-ej-text” attribute. Add the highlighted code to the progress bar div as follows.

{% highlight html %}

<!-- Progressbar control -->

<div style="width: 75%; margin:auto;" >

	<div id="progress" data-role="ejmprogress" data-ej-value="73" data-ej-enablecustomtext=true data-ej-text="Installing...">

	</div>
	
</div>

{% endhighlight %}

Run this code and you will see the below output.

![](Getting-Started_images/Getting-Started_img4.png)

## Customize the text and value dynamically

The progress bar text and its value can be changed dynamically. In our scenario to indicate the progress of installation, its value dynamically changes when you click the install button. And when it reaches 100%, then the progress bar text will change from “Installing…” to “Complete…” Here its value must start from 0, so the data-ej-value attribute is removed and the script codes are modified as follows

{% highlight html %}

<!-- Progressbar control -->

<div style="width: 75%; margin:auto;" >

	<div id="progress" data-role="ejmprogress"  data-ej-enablecustomtext=true data-ej-text="installing..." > 

          <!-- data-ej-value=”73” is removed here -->

	</div>

</div>

{% endhighlight %}

You can use JavaScript “setInterval” function to change its value and text dynamically.

{% highlight js %}

window.currValue = 0;

$(function () {

	window.progressObject = $("#progress").data("ejmProgress"); // create object for progressbar

	$("#progress").hide(); //to hide progressbar at starting

});

function startProgress(args) {

	$(".e-m-btnwrapper").hide(); //to hide button

	$("#progress").show(); // to show progressbar

	window.timeInterval = setInterval(runProgress, 100); //set time intervel to repeat the process

}

function runProgress() {

	progressObject.option("value", window.currValue); //set value for progress

	var value = currValue++;

	if (value == 100) {

		progressObject.option("text", "Completed..."); // change the text when it reaches 100%

		clearInterval(window.timeInterval); //to clear time interval

	}

}

{% endhighlight %}

Run this code and you will see the following output after clicking the install button. This output is taken after the progress bar value reaches 100%. The text of the progress bar is changed in the below output. 

![](Getting-Started_images/Getting-Started_img5.png)

## ProgressBar event handling 

From the above steps, you have learnt how to create and customize Essential JavaScript Mobile Progress bar widget with use case samples. You can have more customization properties other than the one used here. To know more about the properties in Mobile Progress bar widget, refer the complete documentation page for Progress bar widget.