---
layout: post
title: Getting Started | Numeric Textbox | Mobilejs | Syncfusion
description: getting started
platform: Mobilejs
control: Numeric Textbox (Mobile)
documentation: ug
---

# Getting Started

In this section you can learn how to create your first Numeric Textbox Control Mobile application.

## Create your first Numeric Textbox in JavaScript

The following is an example for Rooms Availability Check and it describes how simple it is to create the first layout of Numeric Textbox and how efficient it is to use the features of the control.

### Create the required layout

You can render the Numeric Textbox control based on the default values for all the properties. You can easily customize Numeric Textbox control by changing its properties according to your requirements.

1. Create an HTML file and add the following template to the HTML file for Rooms availability check form creation.

  {% highlight html %}
   
	   <!DOCTYPE html>
	   <html>
		   <head>
			   <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
			   <title>Rooms Availability Check</title>
			   <link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
			   <script src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>
			   <script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"> </script>
		   </head>
		   <body>
			   <!--Page Header-->
			   <div data-role="ejmheader" data-ej-title="Rooms Availability" data-ej-position="fixed" id="page_header"></div>
				<div id="content" class="content">
					<div class="content_area">
						<!--Numeric TextBox 1 code here-->
						<!--Numeric TextBox 2 code here-->
						<div class="text_row button_cnt">
							<input data-role="ejmbutton" data-ej-text="Check Availability" type="button" id="but_submit"/>
						</div>
					</div>
				</div>
		   </body>
	   </html>
	   
{% endhighlight %}

2. To render Numeric Textbox control, specify ejmnumeric as the date-role attribute for an &#60;input&#62; element and type the attribute as number. Add the following code example to render numeric textbox to input the number of persons per room.
   
{% highlight html %}
   
	   <!--Numeric TextBox 1 code-->
	   
	   <div class="text_row">
		
			<label>No of person per room :</label>
		   
			<input data-role="ejmnumeric" data-ej-watermarktext="1" data-ej-showspinbutton="true" data-ej-minvalue="1" data-ej-maxvalue="6" type="number" name="person" id="persontext" />
	   
	   </div>
   
{% endhighlight %}
   
3. Add the following code example to render the Numeric Textbox to input number of rooms needed.
   
{% highlight html %}
   
	   <!--Numeric TextBox 2 code-->
	   
	   <div class="text_row">
	   
		   <label>No of rooms :</label>
		   
		   <input data-role="ejmnumeric" data-ej-watermarktext="1" data-ej-showspinbutton="true" data-ej-minvalue="1" data-ej-maxvalue="5" type="number" name="rooms" id="roomstxt" />
	   
	   </div>
{% endhighlight %}
   
4. To improve the look and feel of Rooms Availability Check you need to add the following code example in your application.

{% highlight css %}
   
	   .content_area {
	   margin-top: 45px;
	   padding: 20px;
	   }
	   
	   .content {
	   max-width: 480px;
	   margin: 0 auto;
	   }
	   
	   .text_row {
	   margin-top: 25px;
	   }
	   
	   .button_cnt {
	   width: 160px;
	   margin-left: auto;
	   margin-right: auto;
	   }
	   
{% endhighlight %} 

   ![](Getting-Started_images/Getting-Started_img1.png)