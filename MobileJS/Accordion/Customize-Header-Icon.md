---
layout: post
title: Customize expand and collapse icon | Accordion | Mobilejs | Syncfusion
description: customize header icon
platform: Mobilejs
control: Accordion (Mobile)
documentation: ug
keywords: accordion, expand, collapse
---

# Customize expand and collapse icon

The “data-ej-showheadericon” attribute is used to display the expand and collapse icon for the Accordion header. 

{% highlight html %}

<div id="accordion_sample" data-role="ejmaccordion" data-ej-showheadericon="true">

     <ul>

         <li data-ej-text="MVC">

            <div>

            Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it. The model consists of application data, business rules, logic, and functions

             </div>

         </li>

         <li data-ej-text="WPF" >

            <div>

             Developed by Microsoft, the Windows Presentation Foundation (or WPF) is a computer-software graphical subsystem for rendering user interfaces in Windows-based applications.

            </div>

         </li>              

         <li data-ej-text="WCF" >

            <div>

            WCF is a tool often used to implement and deploy a service-oriented architecture (SOA). It is designed using service-oriented architecture principles to support distributed computing where services have remote consumers.

             </div>

         </li>  

    </ul>

</div> 

{% endhighlight %}

The following screenshot displays header icon.

![](Customize-Header-Icon_images/Customize-Header-Icon_img1.png)