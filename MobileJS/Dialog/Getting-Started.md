---
layout: post
title: getting-started
description: getting started
platform: js
control: Dialog
documentation: ug
keywords: dialog
---

# Getting started

This section explains briefly on how to create a Dialog control in your application.

## Create your first Dialog in JavaScript

The EssentialJavaScriptDialog window is an overlay positioned and displays a message along with supplementary content such as images or text and interactive content such as forms, etc.  It contains a title and a content area. 

Create the required layout

You can render the Dialog control based on the default values for all the properties. You can easily customize Dialog control by changing their properties according to your requirements.

1. Create an HTML file and add the following template to the HTML file for Mailsignin form creation.

2. Create an HTML file and add the following template code snippets. 

{% highlight html %}

<html>
<head>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <title>ListView</title>
    <link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js"></script>
    <script src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js"></script>
    <script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"></script>
</head>
<body>
    <div>
        <!--Add Control rendering code here-->
    </div>
</body>
</html>



{% endhighlight %}

Add the below HTML code

{% highlight html %}

<div id="alertdlg" data-role="ejmdialog" data-ej-title="Low Battery" data-ej-mode="alert"
            data-ej-leftbuttoncaption="Dismiss" data-ej-enablemodal="true" data-ej-enableautoopen="false"
            data-ej-buttontap="alertClose">
            <div>
                10% of battery remaining
            </div>
        </div>
        <div style="text-align: center">
            <input data-role="ejmbutton" data-ej-text="Click here to open dialog" type="button" data-ej-touchend="openAlertDialog" id="btn1" />
        </div>


{% endhighlight %}

Add the Script

{% highlight js %}

function alertClose(args) {
            $("#alertdlg").ejmDialog("close");
        }
        function openAlertDialog(args) {
            $("#alertdlg").ejmDialog("open");
        }


{% endhighlight %}

![](Getting-Started_images\create-your-first-dialog-in-javascript_img1.png)


