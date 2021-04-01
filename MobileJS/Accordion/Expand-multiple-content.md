---
layout: post
title: Expand multiple content | Accordion | Mobilejs | Syncfusion
description: expand multiple content
platform: Mobilejs
control: Accordion (Mobile)
documentation: ug
keywords: accordion, multipleopen
---

# Expand multiple content

The data-ej-enablemultipleopen attribute is used to display or expand more than one item at a time. The index of the items to be expanded can be specified by using data-ej-selecteditems attribute as an array.

{% highlight html %}

<div id="accordion_sample" data-role="ejmaccordion" data-ej-enablemultipleopen="true" data-ej-selecteditems="[0,1]">

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

The following screenshot displays expand multiple contents:

![](Expand-multiple-content_images/Expand-multiple-content_img1.png)