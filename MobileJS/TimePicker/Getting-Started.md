---
layout: post
title: Getting Started | TimePicker | Mobilejs | Syncfusion
description: getting started
platform: Mobilejs
control: TimePicker (Mobile)
documentation: ug
---

# Getting Started

The TimePicker widget displays a TimePicker in your web page and allows you to pick a time value from it. This section explains on how to customize two TimePickers for a real time hotel reservation scenario.

The below screenshot illustrates the usage of TimePickers in the hotel reservation scenario.

![](Getting-Started_images/Getting-Started_img1.png)

## Create the necessary Layout

Create an Essential JavaScript Mobile TimePicker widget easily by using a simple input element.

Create an HTML file and add the following code example to it.

{% highlight html %}

<!DOCTYPE html>
<html>
<head>
    <title> TimePicker </title>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <link href="[http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css](http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css)" rel="stylesheet" />
    <script src="[http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js](http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js)"></script>
    <script src="[http://cdn.syncfusion.com/js/assets/external/jsrender.min.js](http://cdn.syncfusion.com/js/assets/external/jsrender.min.js)"></script>
    <script src="[http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js](http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js)"></script>
</head>
<body>
    <!-- header control -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Hotel Reservation" data-ej-isrelative="true" data-ej-titlealignment="center"></div>
    <div align="center">
        <table>
            <tr>
                <td class="tdclass">Date</td>
                <td class="innerclass">
                    <span class="innerdp">
                        <!-- create datepicker to select booking date -->
                        <input id="entryDate" data-role="ejmdatepicker" />
                    </span>
                </td>
            </tr>
            <tr>
                <td class="tdclass">In Time</td>
                <td class="innerclass">
                    <span class="innerdp">
                        <!-- Add InTime Timepicker element here -->
                    </span>
                </td>
            </tr>
            <tr>
                <td class="tdclass">Out Time </td>
                <td class="innerclass">
                    <span class="innerdp">
                        <!-- OutTime Timepicker element -->
                    </span>
                </td>
            </tr>
        </table>
        <!-- button to confirm the reservation -->
        <input type="button" data-role="ejmbutton" data-ej-text="Book Now" data-ej-rendermode="auto" id="btnbook" data-ej-touchend="displayConfirmation" />
    </div>
</body>
</html>

{% endhighlight %}

Add the following styles to display the TimePicker’s input element.

{% highlight css %}

<style type="text/css">
	
.tdclass {
    width: 100px;
}

td {
    padding: 8px;
}

table {
    margin: 10px;
}

.innerclass {
    width: 300px;
}
</style>

{% endhighlight %}


## Create a TimePicker

To render the TimePicker control, set `data-role` attribute to `ejmtimepicker` to the specific input element as follows.

{% highlight html %}

<!-- InTime Timepicker element -->
<input id="startTime" data-role="ejmtimepicker" />

<!-- OutTime Timepicker element -->
<input id="endTime" data-role="ejmtimepicker" />

{% endhighlight %}

Execute the above code example and focus on **InTime** or **OutTime** TimePicker element to render the following output.

![](Getting-Started_images/Getting-Started_img2.png)

## Set the hour format

The TimePicker widget supports both 12 hour and 24 hour time format. The default value is 24 hour format. In this application, the booking table opens for all time throughout the day. Refer to the following code example to set 12 hour format by using the `data-ej-hourformat` attribute. 

{% highlight html %}

 <!-- InTime Timepicker element -->
<input id="startTime" data-ej-hourformat="twelve" data-role="ejmtimepicker"/>

  <!-- OutTime Timepicker element -->
<input id="endTime" data-ej-hourformat="twelve" data-role="ejmtimepicker"/>

{% endhighlight %}

Execute the above code example and focus on **InTime** or **OutTime** TimePicker element to render the following output.

![](Getting-Started_images/Getting-Started_img3.png)

Refer to the following code example to display a confirmation message on clicking the **Book Now** button handled by the button's touch end event.

{% highlight html %}

<div id="alertdlg" data-role="ejmdialog" data-ej-title="Booking Confirmation" data-ej-mode="alert" data-ej-leftbuttoncaption="OK" data-ej-enablemodal=true data-ej-enableautoopen=false data-ej-buttontap="alertClose">
    <div>Hotel reserved for specified time</div>
</div>
		
{% endhighlight %}

Add the following code example

{% highlight js %}

<script type="text/javascript">
	
function alertClose() {
	$("#alertdlg").ejmDialog("close"); //To close dialog
}

function displayConfirmation(args) {
	App.activePage.find("#alertdlg").ejmDialog("open"); //To open dialog
}

</script>

{% endhighlight %}

Execute the above code and click the **Book Now** button to display the confirmation message as illustrated in the following screenshot.

![](Getting-Started_images/Getting-Started_img4.png)