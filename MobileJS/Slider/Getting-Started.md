---
layout: post
title: Getting-Started | Slider | Mobilejs | Syncfusion
description: getting started 
platform: js
control: Slider
documentation: ug
keywords: slider, range, events
---

# Getting started 

**Essential JavaScript Mobile Slider** provides the selection of a single value or a range of values, using an interface with sliding handles.  The following example shows you how to create a **Shopping Cart App** and through that learn the features in the Slider widget.


![](Getting-Started_images/Getting-Started_img1.png) 

## Create the layout for shopping cart app

**Essential JS Mobile Slider** widget is rendered by a <div> element with its required properties. You can customize Slider control by changing its properties according to your requirements. In the **Shopping Cart App **, the **Range Slider** is used to set the **price range**.


Create an **HTML** file and add the following template to the HTML file.


{% highlight html %}

<!DOCTYPE html>
<html>
<head>
    <title>Slider</title>
    <link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>
    <script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"> </script>
</head>
<body>
    <div id="page" data-role="appview">
        <!-- header control -->
        <div data-role="ejmheader" data-ej-title="Shopping cart">
        </div>	
        <div id="content">
            <div id="form" style="margin: 20px;">
                <div>
                    <div>
                        <span class="text">Search-->MobilePhones-->Filter</span>
                    </div>
                    <br>
                    <span class="text">Operating System</span>
                </div>
                <!-- create check box for different OS  -->
                <div align="center" id="checkbox" style="margin-bottom: 10px">
                    <table border="0" cellpadding="6">
                        <tr>
                            <td>
                                <input id="ios" name="chkbox" data-role="ejmcheckbox" />IOS</td>
                            <td>
                        </tr>
                        <tr>
                            <td>
                                <input id="android" name="chkbox" data-role="ejmcheckbox" />Android</td>
                        </tr>
                        <tr>
                            <td>
                                <input id="windows" name="chkbox" data-role="ejmcheckbox" />Windows</td>
                            <td>
                        </tr>
                    </table>
                </div>
                <div style="margin-bottom: 10px">
                    <span class="text">Price Range</span>
                </div>
                <span id="minvalue" style="float: left;"></span>
                <span id="maxvalue" style="float: right;"></span>
                <div style="margin-top: 35px;">
                 <!—Add Slider control here-->      
                </div>
                <div align="center" style="margin-top: 20px;">
                    <input type="button" data-role="ejmbutton" data-ej-text="Submit" id="button" data-ej-touchend="ShowDialog" />
                </div>
                <!-- dialog control -->
                <div id="alertdlg" data-role="ejmdialog" data-ej-title="Dialog" data-ej-leftbuttoncaption="OK" data-ej-buttontap="alertClose">
                    <div id="dialogContent">Based on your suggestion the phones will displayed now     </div>
                </div>
            </div>
        </div>
        <!-- ScrollPanel -->
        <div data-role="ejmscrollpanel" data-ej-target="content"></div>
    </div>
    <style type="text/css">
        span.text {
            font-size: 15px;
            font-weight: bold;
        }
    </style>
</body>
</html>


{% endhighlight %}

Execute the above code example to render the following output.

![](Getting-Started_images/Getting-Started_img2.png) 



## Create Slider control

To render Slider control, set **ejmslider** to data-role attribute to <div> element. Set 100 as the minimum value for the Slider using data-ej-minvalue, and set 5000 as the maximum value using data-ej-maxvalue. Set data-ej-incrementstep to 100 so that the slider is moved for every 100 values. 

{% highlight html %}

<!-- Slider control -->

 <div id="slider" data-role="ejmslider" data-ej-minvalue="100" data-ej-maxvalue="5000" data-ej-incrementstep="100"></div>

{% endhighlight %}


Run the above code example to render the following output.

![](/mobilejs/Slider/Getting-Started_images/Getting-Started_img3.png) 


## Create the Range Slider

You can set the price range using Range Slider. Set **data-ej-enablerange** attribute to “True”. You can set the initial range values by using data-ej-values attribute. Here, you can set the values as [300, 1500]. The Slider’s left thumb is set to 300 and the right thumb is set to **1500**. 		

Add the following code to the **Slider <div>**.
 
{% highlight html %}

<!-- Slider control -->

<div id="slider" data-role="ejmslider" data-ej-minvalue="100" data-ej-maxvalue="5000" data-ej-enablerange="true" data-ej-values="[300,1500]" data-ej-incrementstep="100"></div>

{% endhighlight %}


Run the above code example to render the following output.

![](Getting-Started_images/Getting-Started_img4.png) 


## Handle events

In this scenario, when you change the Slider value, the corresponding values are updated to the <span> element that acts as a label for Slider. You can use data-ej-slide event that is handled by appropriate function 		

Add the following code to the **Slider <div>**.
 
{% highlight html %}

<!-- Slider control -->

<div id="slider" data-role="ejmslider" data-ej-minvalue="100" data-ej-maxvalue="5000" data-ej-enablerange="true" data-ej-values="[300,1500]" data-ej-slide="processOnSlide" data-ej-incrementstep="100"></div>

{% endhighlight %}

From the Slider’s getValue API, you can get the present value of both the Slider handles, anytime. Add the following code example to the <script> tag. 

{% highlight html %}
//to display the slider value in span element (label) at initialize
        $(function (args) {
            window.dialogObject = $("#alertdlg").data("ejmDialog"); //to create dialog object
            window.sliderObject = $("#slider").data("ejmSlider"); //to create slider object
            setValue("300,1500");//set slider labels at initialize 
          });
        // handling slider slide event
        function processOnSlide() {
            var value = sliderObject.getValue();// get the value of slider by using getValue API
            setValue(value);
        }
        function setValue(value) {
            var position = value.split(",");
            $("#minvalue").html("$" + position[0]); //to set left thumb value to the left span
            $("#maxvalue").html("$" +position[1]); // to set right thumb value to the right span
        }
        }


{% endhighlight %}

Run the above code example to render the following output.

![](Getting-Started_images/Getting-Started_img1.png) 

In this scenario, a dialog is displayed to provide information about the search when Submit is clicked. Add the following code to the  ** <script>** tag.


{% highlight html %}
//to display the slider value in span element (label) at initialize
//to open dialog
        function ShowDialog(args) {
            dialogObject.open(); //to show dialog
        } 
        //to close dialog
        function alertClose(args) {
            dialogObject.close(); //close dialog
        }

{% endhighlight %}


Execute the above code example to render the following output, when you click Submit.

![](Getting-Started_images/Getting-Started_img-5.png) 