---
layout: post
title: API Configuration | Introduction | Mobilejs | Syncfusion
description: api configuration
platform: Mobilejs
control: Introduction
documentation: ug
---

# API Configuration

It is possible to get and set the various properties available within the controls after its creation.

## Getting API values

The API values can be accessed/retrieved by using either of the following ways.


{% highlight javascript %}

1. $("jquery-selector").<ejm-plugin-name>("model.propertyName");

Example:  $("#myDate").ejmDatePicker("model.dateFormat");


2. $("jquery-selector").<ejm-plugin-name>("option", "propertyName");

Example:  $("#myDate").ejmDatePicker("option", "dateFormat");

{% endhighlight %}


## Setting values to the API

It is possible to set new values to the properties of the Syncfusion widgets during or after the control initialization as described. 

### During Initialization

{% highlight javascript %}

1. <<HtmlTag> data-role="<ejm-plug-in-name>" data-ej-"<propertyName>"= "<value>"/> **[Recommended method]**

Example:  <input id="myDate" data-role="ejmdatepicker" data-ej-value="01/01/2000" />

2. $("jquery-selector").<ejm-plugin-name>({ propertyName1 : value1, propertyName2: value2, … });

Example:  $("#myDate").ejmDatePicker({ value: "01/01/2015", dateFormat: "MM/dd/yyyy" });

{% endhighlight %}

### After initialization

{% highlight javascript %}

1. var obj = $("jquery-selector").data("<ejm-plugin-name>");  **[Recommended method]**

obj.option({ propertyName: value });

Example:  var dateObject = $("#myDate").data("ejmDatePicker");

         dateObject.option({ dateFormat: "dd/MM/yyyy" });

2. $("jquery-selector").<ejm-plugin-name>("model.propertyName", "value");

Example:  $("#myDate").ejmDatePicker("model.dateFormat", "dd/MM/yyyy" );

3. $("jquery-selector").<ejm-plugin-name>("option", "propertyName", "value");

Example:  $("#myDate").ejmDatePicker("option", "dateFormat", "dd/MM/yyyy");


{% endhighlight %}