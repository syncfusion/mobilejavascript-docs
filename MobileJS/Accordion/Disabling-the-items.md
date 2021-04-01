---
layout: post
title: Disabling the items | Accordion | Mobilejs | Syncfusion
description: disabling the items
platform: Mobilejs
control: Accordion (Mobile)
documentation: ug
keywords: accordion, disble, disableditems
---

# Disabling the items

The data-ej-disableditems attribute is used to disable one or more specified items by using its index that can be given as an array.

{% highlight html %}

<div id="accordion_sample" data-role="ejmaccordion" data-ej-disableditems="[1]">

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

The following screenshot displays disabling items:

![](Disabling-the-items_images/Disabling-the-items_img1.png)