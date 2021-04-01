---
layout: post
title: Invoking Methods | Introduction | Mobilejs | Syncfusion
description: invoking methods
platform: Mobilejs
control: Introduction
documentation: ug
---

# Invoking Methods

The functions can be invoked the same way the properties are accessed. The following syntaxes define the ways to invoke the public methods of the widgets.

{% highlight javascript %}

1. var obj = $("jquery-selector").data("<ejm-plugin-name>"); **[Recommended method]**

obj.methodName(param1, param2, param3, ...)

Example: 
        var lwObject = $("#btn").data("ejmListView");
        lwObject.selectItemByIndex(2);


2. $("jquery-selector").<ejm-plugin-name>("methodName");

Example:  
        $("#button").ejmButton("disable");

3. $("jquery-selector").<ejm-plugin-name>("methodName", "param1", "param2", …);

Example:  
        $("#listview").ejmListView("selectItemByIndex", 2);

{% endhighlight %}