---
layout: post
title: Getting-Started | Textbox | Mobilejs | Syncfusion
description: getting started 
platform: js
control: Text Box
documentation: ug
keywords: textbox
---

# Getting Started 

   The **Essential JavaScript Mobile Textbox** is used to display or get any value.To create a textbox for the login page in the mobile application, follow the guidelines given. 

![](Getting-Started_images/Getting-Started_img1.png) 

## Create the layout

Create an **HTML** file and add the following template to the HTML file.


{% highlight html %}

<!DOCTYPE html>
<html>
<head>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <title>Textbox</title>
    <link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>
    <script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"> </script>
</head>
<body>
    <!--Header Control-->
    <div data-role="ejmheader" id="mailheader" data-ej-title="Login"></div>
    <div class="sample" style="padding: 62px 15px">
        <div class="frame">
            <div class="control">
                <table class="editors">
                    <tbody>
                        <tr>
                            <td>
                                <label>
                                    Name
                                </label>
                            </td>
                            <td>
                                <!--Add Textbox control-->
                            </td>
                        </tr>
                        <tr>
                            <td>
                                <label>
                                    Password
                                </label>
                            </td>
                            <td>
                                <!--Password Control-->
                            </td>
                        </tr>
                    </tbody>
                </table>
                <center>
                    <div class="button">
                        <!--Button Control-->
                        <input type="button" data-role="ejmbutton" data-ej-text="Login" />
                    </div>
                </center>
            </div>
        </div>
    </div>
    <style type="text/css">
        td {
            padding: 9px;
        }
    </style>
</body>
</html>

{% endhighlight %}

## Add Textbox Control

To create the Textbox control add the following code.

Execute the above code example to render the following output.

{% highlight html %}

<!--Add Textbox control-->

<input id="textbox_sample" data-role="ejmtextbox" data-ej-watermarktext="User Name"  data-ej-width="200"/>
  <!--Password Control-->

<input id="password" data-role="ejmpassword" data-ej-watermarktext="Password" data-ej-width="200" />


{% endhighlight %}

Run the code and get the following output.

![](Getting-Started_images/Getting-Started_img1.png) 



