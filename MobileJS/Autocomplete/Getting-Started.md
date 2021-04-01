---
layout: post
title: Getting-Started
description: create your first autocomplete text box in javascript
platform: js
control: Overview
documentation: ug
---

# Getting Started

## Create your first AutoComplete Text box in JavaScript

Essential JavaScript Mobile Autocomplete control can be rendered using a simple HTML textbox. It is rendered based on the default values for all the properties and you can easily customize this control by changing its properties. The following code snippets shows examples of how to search contact using Mobile Autocomplete. 

![](Getting-Started_images\Getting-Started_1.png)





Create an HTML file and add the following template code snippets to create Autocomplete control.


{% highlight html %}

<!DOCTYPE html>
<html>   
<head>
<title> Autocomplete</title>
<link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet"/>
<script src="http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js"></script>
<script src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
<script src="http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js"></script>
<script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"></script>

<script src="http://js.syncfusion.com/UG/Mobile/Content/contacts.min.js"></script>
</head>

<body>
    <!-- Header control -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Contacts" data-ej-isrelative="true">
    </div>
    <div id="content" style="padding:10px;">
        <div style="padding: 5px 0; text-indent: 5px;">
            Select Contacts
        </div>
        <div>
            <!--Add Autocomplete Elements here.-->
        </div>
    </div></body>
</html>


{% endhighlight %}



To render the Autocomplete control, set “data-role” attribute to “ejmautocomplete” to an input element. 



{% highlight html %}


     <!-- Autocomplete control -->
     <input id="contacts" data-role="ejmautocomplete" />



{% endhighlight %}





You can customize its watermark text using data-ej-watermarktext attribute.

{% highlight html %}


<!-- Autocomplete control -->
<input id="contacts" data-role="ejmautocomplete" data-ej-watermarktext="Search Contacts" />



{% endhighlight %}



![](Getting-Started_images\Getting-Started_2.png)


## Data binding

To add data source to Autocomplete control, you can set data-ej-datasource attribute value with the particular data source name. You need to assign the necessary column (field) name of the data source to data-ej-fields-text attribute.

{% highlight html %}


     <!-- Autocomplete control -->
     <!-- The data source "window.contacts" is referred from contacts.min.js-->
     <input id="contacts" data-role="ejmautocomplete"
     data-ej-watermarktext="Search Contacts" data-ej-datasource="window.contacts" data-ej-fields-text ="name"/>



{% endhighlight %}



![](data-binding_images\data-binding_img1.png)


## Event handling

The data-ej-select attribute enables you to handle Autocomplete selection event, by assigning a function name to the attribute. In this case, you can set data-ej-select attribute with the function name OnSelect.  By executing the onSelect( ) function you can implement necessary action to show the full contact details of the selected contact name.

{% highlight html %}

             <!-- Autocomplete control -->
    <input id="contacts" data-role="ejmautocomplete" data-ej-watermarktext="Search Contacts" data-ej-datasource="window.contacts" data-ej-fields-text="name" data-ej-enablemultiselect="true" data-ej-delimiterchar=";" data-ej-select="onSelect" />

     <!-- onSelect() function is called on selection of a suggestion item.-->

     <!-- Dialog control -->
     <div id="dialog" data-role="ejmdialog" data-ej-title="Alert" data-ej-enablemodal=true
         data-ej-leftbuttoncaption="OK" data-ej-buttontap="hidedialog">
        <div id="dialogcontent"><!-- Dialog content --></div>
     </div>



{% endhighlight %}



Add the following script.

{% highlight js %}

function onSelect(args) {
            //Actions that are performed on selection
            $("#dialogcontent").html(args.text + " was selected");
            var dialogobj = $("#dialog").data("ejmDialog");
            dialogobj.open();
        }
        function hidedialog(e) {
            //Hides dialog
            var dialogobj = $("#dialog").data("ejmDialog");
            dialogobj.close();
        } 


{% endhighlight %}


![](Getting-Started_images\event-handling_img1.png)


