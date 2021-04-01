---
layout: post
title: Customize content height | Accordion | Mobilejs | Syncfusion
description: customize content height
platform: Mobilejs
control: Accordion (Mobile)
documentation: ug
keywords: accordion, height
---

# Customize content height

The data-ej-heightadjustmode attribute is used to customize the height of each item’s content. It specifies the height style of the Accordion.  Set the “data-ej-heightadjustmode” attribute with the following possible values.

* Content - This mode fits the height based on the content in the panel. 
* Auto - This mode sets the height based on the largest content in the panel.
* Fill - It automatically sets the dimensions of each Accordion item to the height of its parent container, that is, to fill the vertical space allocated by its container.



{% highlight html %}

<div id="accordion_sample" data-role="ejmaccordion" data-ej-heightadjustmode="auto">

            <ul>

                <li data-ej-text="MVC">

                    <div>

                     Model-view-controller (MVC) is a software architecture pattern which separates the representation of information from the user's interaction with it. The model consists of application data, business rules, logic, and functions

                    </div>

                </li>

                <li data-ej-text="WPF">

                    <div>

                        Developed by Microsoft, the Windows Presentation Foundation (or WPF) is a computer-software graphical subsystem for rendering user interfaces in Windows-based applications.

                    </div>

                </li>

                <li data-ej-text="WCF">

                    <div>

                        WCF is a tool often used to implement and deploy a service-oriented architecture (SOA). It is designed using service-oriented architecture principles to support distributed computing where services have remote consumers.

                    </div>

                </li>	

            </ul>

        </div>

{% endhighlight %}

The following screenshot displays the customized "auto" content height.

![](Customize-content-height_images/Customize-content-height_img1.png)