---
layout: post
title: Getting Started | DatePicker | Mobilejs | Syncfusion
description: getting started
platform: Mobilejs
control: DatePicker (Mobile)
documentation: ug
---

# Getting Started

The DatePicker control provides support for displaying DatePicker calendar in a web page and also allows the user to pick or directly enter the date value in it. 

By following the below guidelines, you can learn how to customize two DatePickers for a real-time ticket booking scenario. The following screenshot demonstrates the ticket booking scenario where the DatePickers are employed.

![](Getting-Started_images/Getting-Started_img1.png)



## Create a DatePicker

You can create a DatePicker widget easily by using simple input element. 

Create an HTML file and add the following code example to it.

{% highlight html %}

<!DOCTYPE html>
<html>
<head>
    <title>Ticket Booking</title>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <link href="[http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css](http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css)" rel="stylesheet" />
    <script src="[http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js](http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js)"></script>
    <script src="[http://cdn.syncfusion.com/js/assets/external/jsrender.min.js](http://cdn.syncfusion.com/js/assets/external/jsrender.min.js)"></script>
    <script src="[http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js](http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js)"></script>
</head>
<body>
    <div>
        <div id="header" data-role="ejmnavigationbar" data-ej-title="Ticket Booking" data-ej-isrelative="true" data-ej-titlealignment="center"></div>
        <!--Add Datepicker element here-->
    </div>
</body>
</html>
	   
{% endhighlight %}

To provide the header title in the layout, set the `data-ej-title` attribute with the desired title value. In this case, you can set it as **Ticket Booking**.

{% highlight html %}

<div id="header" data-role="ejmnavigationbar" data-ej-title="Ticket Booking" data-ej-isrelative="true" data-ej-titlealignment="center"></div>

{% endhighlight %}  

To render the DatePicker control, set the `ejmdatepicker` to `data-role` attribute for the specific input element as follows.

{% highlight html %}

   <table>
        <tr>
            <td class="tdclass">Onward Date</td>
        </tr>
        <tr>
            <td class="tdclass">
                <span class="innerdp">
                    <input id="startDate" data-role="ejmdatepicker" />
                </span>
            </td>
        </tr>
        <tr>
            <td class="tdclass">Return date</td>
        </tr>
        <tr>
            <td class="tdclass">
                <span class="innerdp">
                    <input id="endDate" data-role="ejmdatepicker" />
                </span>
            </td>
        </tr>
   </table>
	 
{% endhighlight %}

Add the following styles to display the DatePicker’s input element.

{% highlight css %}

<style type="text/css">
    .tdclass {
        width: 300px;
        font-weight: bold;
        padding-bottom: 10px;
    }
    table {
        margin: 30px auto;
    }
</style>
	   
{% endhighlight %}
   
Run the above code example, to render the DatePicker.

![](Getting-Started_images/Getting-Started_img2.png)


## Setting Min and Max Date 

In a real-time ticket booking scenario, the booking is open for a limited number of days only. You can select any date, only in that range. This can be achieved by using the attributes `data-ej-mindate` and `data-ej-maxdate`. 

The following code helps you to set the mindate and maxdate.

{% highlight js %}

<script type="text/javascript">
	
var curDate = new Date();// Mention the current date.

// The following code mentions 2 years from the current date.
var rangeDate = new Date(curDate.getFullYear() + 2, curDate.getMonth(), curDate.getDate());

// Sets minDate and maxDate at the time of document ready.
$(function () {
	var startdate = $("#startDate").data("ejmDatePicker");
	startdate.option({ "minDate": curDate, "maxDate": rangeDate });
	var enddate = $("#endDate").data("ejmDatePicker");
	enddate.option({ "minDate": curDate, "maxDate": rangeDate });
});

</script>

{% endhighlight %}

Run the above code example to render a DatePicker with Min and Max Date as shown in the below image.

![](Getting-Started_images/Getting-Started_img3.png)

## Validations on Min and Max Date Values

You can select Onward journey date in the first DatePicker. The Return journey date is selected in second date picker after selecting Onward journey date. This validation process is done after the selection of Onward journey date and the changes are reflected on the Return journey date selection DatePicker. Manipulate this process by using the **select** event of Onward journey date DatePicker by using `data-ej-select` attribute. 

The following code example explains how to set an event to process the Min and Max Date Validations.

{% highlight html %}

   <table>
        <tr>
            <td class="tdclass">Onward Date</td>
        </tr>
        <tr>
            <td class="tdclass">
                <span class="innerdp">
                    <input id="startDate" data-role="ejmdatepicker" data-ej-select="validateMinDateForReturn" />
                </span>
            </td>
        </tr>
        <tr>
            <td class="tdclass">Return date</td>
        </tr>
        <tr>
            <td class="tdclass">
                <span class="innerdp">
                    <input id="endDate" data-role="ejmdatepicker" />
                </span>
            </td>
        </tr>
    </table>

{% endhighlight %}

The `select` event is handled by the user-defined `validateMinDateForReturn` function as follows.

{% highlight js %}

<script type="text/javascript">

function validateMinDateForReturn (args) {
	var selDate = new Date(args.value); // Mentions the selected date.
	minDatepicker = $("#endDate").data("ejmDatePicker");// Creates DatePicker object
	minDatepicker.option({ "minDate": selDate });// Sets minDate property through setModel of DatePicker object.
}

</script>

{% endhighlight %}

The above code example outputs the following image.

![](Getting-Started_images/Getting-Started_img4.png)