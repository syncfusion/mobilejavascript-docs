---
layout: post
title: Wiring Events | Introduction | Mobilejs | Syncfusion
description: wiring events
platform: Mobilejs
control: Introduction
documentation: ug
---

# Wiring Events

Whenever the control undergoes some changes or action, it should be notified to the users properly. To notify such actions, the appropriate events should be bound to the control. Events are wired the same way as jQuery events are bound, either during or after control initialization.

## During Initialization



{% highlight javascript %}

$(“jquery-selector”).<ejm-plugin-name>({ eventName : <eventhandler> });

Example:  

        $("#myDate").ejmDatePicker({
            select: function () {
                // Event handler 
            }
        });

{% endhighlight %}

## After initialization

 

{% highlight javascript %}

$(“jquery-selector”).<ejm-plugin-name>("model.eventName", <eventhandler>);

Example: 

$("#myDate").ejmDatePicker("model.select" , function () {

	// Event handler

 });
		 

{% endhighlight %}