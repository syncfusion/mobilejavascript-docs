---
layout: post
title: Getting started | Accordion | Mobilejs | Syncfusion
description: getting started
platform: Mobilejs
control: Accordion (Mobile)
documentation: ug
keywords: accordion, collapse
---

# Getting started

## Create your first Accordion in JavaScript

Essential JavaScript Accordion provides a way to display collapsible content panels to present information in a limited amount of space. In the following guidelines, you can learn to create a Live Soccer App and through that you can learn about the features in Accordion widget.

![](Getting-Started_images/Getting-Started_img1.png)

In the above screenshot, you can click headers to expand/collapse content. You can also load content on demand, by specifing the URL to be loaded.



## Create the required layout

Essential JavaScript Accordion widget is rendered, either by specifying static content, or by using on demand contents by specifying the respective URL. Either case, Accordion control is rendered based on the default values for all the properties; you can easily customize Accordion control by changing its properties according to your requirements. In the Live Soccer App, three panels are required; one for displaying the Recent Matches, second for listing out the Upcoming Matches and another for displaying the Ongoing Match Updates on the Live Soccer App. The following steps will guide you to create a basic Accordion for your application.

Create an HTML file and add the following template to the HTML file to create Accordion.

{% highlight html %}

<!DOCTYPE html>

<html>

<head>

    <title>Accordion</title>
    <link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>
    <script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"> </script>
 </head>

<body>

    <div id="page" data-role="appview">

        <div id="header" data-ej-title="Live Soccer" data-role="ejmheader"></div>

        <div id="accordion" class="sample">

            <div>

                <!--Add Accordion Elements here.-->

            </div>

        </div>

        <!--Scroll Panel-->

        <div data-role="ejmscrollpanel" data-ej-target="accordion"></div>

    </div>

</body>

</html>

{% endhighlight %}

To render Accordion control, set ejmaccordion as data-role attribute to <div> element, and include a list of Accordion items, through <li> element, to be added. Add the data-ej-text attribute to set text for each item.

{% highlight html %}

<!--Accordion Control-->

<div id="accordionControl" data-role="ejmaccordion">

  <ul>

     <!--Accordion Panel 1-->

     <li data-ej-text="Recent Matches">

	     <div>

	          <!--Content-->

	     </div>

     </li>

     <!--Accordion Panel 2-->

     <li data-ej-text="Upcoming Matches">

        <div>

             <!--Content-->

        </div>

     </li>

     <!--Accordion Panel 3-->

     <li data-ej-text="Ongoing Matches">

     </li>

  </ul>

</div>

{% endhighlight %}

Run this code example and you can see the following output.

![](Getting-Started_images/Getting-Started_img2.png)


## Select Accordion item

The data-ej-selecteditems attribute is used to expand the specific content section, initially by using its index value. Multiple content sections can be expanded at a time. It accepts numeric array type. The default value of selecteditems is [0]. So the first panel will be in an expanded state. But in this case example you need all the panels in collapsed state, initially. So you need to set data-ej-selecteditems attribute with the value [-1].

{% highlight html %}

<!--Accordion Control-->

<div id="accordionControl" data-role="ejmaccordion" data-ej-selecteditems="[1]">

	<ul>

		<!--Accordion Panel 1-->

		<li data-ej-text="Recent Matches">

		</li>

        <!--Accordion Panel 2-->

        <li data-ej-text="Upcoming Matches">

        	<div>

                 <!--Content-->

            </div>

       	</li>

		<!--Accordion Panel 3-->

		<li data-ej-text="Ongoing Matches">

		</li>

	</ul>

</div>

{% endhighlight %}

Run this code example and you can see the following output.

![](Getting-Started_images/Getting-Started_img3.png)

## Enable header icons

By default, header icons are  visible. To make the icons invisible, set data-ej-showHeadericon attribute to false.

{% highlight html %}

                <!--Accordion Control-->
                <div id="accordionControl" data-role="ejmaccordion"
                    data-ej-showheadericon="false">
                    <ul>
                        <!--Accordion Panel 1-->
                        <li data-ej-text="Recent Matches"></li>
                        <!--Accordion Panel 2-->
                        <li data-ej-text="Upcoming Matches">
                            <div>
                                <!--Content-->
                            </div>
                        </li>
                        <!--Accordion Panel 3-->
                        <li data-ej-text="Ongoing Matches"></li>
                    </ul>
                </div>

{% endhighlight %}

![](Getting-Started_images/Getting-Started_img4.png)

## Make Accordion collapsible

By default, all the content sections are not collapsible. To make all its content section collapsible, set data-ej-collapseall attribute to true.

{% highlight html %}

<!--Accordion Control-->

    <div id="accordionControl" data-role="ejmaccordion" data-ej-collapseall="true">
                    <ul>
                        <!--Accordion Panel 1-->
                        <li data-ej-text="Recent Matches"></li>
                        <!--Accordion Panel 2-->
                        <li data-ej-text="Upcoming Matches">
                            <div>
                                <!--Content-->
                            </div>
                        </li>
                        <!--Accordion Panel 3-->
                        <li data-ej-text="Ongoing Matches"></li>
                    </ul>
         </div>


{% endhighlight %}

![](Getting-Started_images/Getting-Started_img8.png)

## Add content

In the case example given, the contents of the Recent Matches and Upcoming Matches panels are given as static. In these content panels, the team results and match schedules are listed.

The following code example is used to add Recent Matches and Upcoming Matches panels’ content.

{% highlight html %}

       <!--Accordion Control-->

  <div id="accordionControl" data-role="ejmaccordion">
          <ul>         
             <!--Accordion Panel 1-->
            <li data-ej-text="Recent Matches">
             <div>
             <!--Content-->
                <div class="message-title">Crystal Palace – 3
                    <div class="time-panel">6th May</div></div>
                  <div class="message-title">Liverpool - 3</div>
                  <div class="text-panel">Match Drawn
                  </div>
                <div class="border-panel"></div>
                <div class="message-title">Arsenal – 1
                    <div class="time-panel">4th May</div></div>
                  <div class="message-title">West Brom - 0</div>
                  <div class="text-panel">Arsenal won the match
                  </div>
                <div class="border-panel"></div>
                <div class="message-title">Rayo – 0
                    <div class="time-panel">3rd May</div></div>
                  <div class="message-title">Athletic - 3</div>
                  <div class="text-panel">Athletic won the match
                  </div>
              </div>
            </li>
              <!--Accordion Panel 2-->                           
             <li data-ej-text="Upcoming Matches">
              <div>
                <!--Content-->
                  <div class="message-title">Man City
                      <div class="time-panel">8th May</div></div>
                    <div class="text-panel">vs</div>
                    <div class="message-title">Aston Villa
                    </div>
                  <div class="border-panel"></div>
                  <div class="message-title">Valladolid
                      <div class="time-panel">8th May</div></div>
                   <div class="text-panel">vs</div>
                   <div class="message-title">Real Madrid
                    </div>
                  <div class="border-panel"></div>
                  <div class="message-title">Villarreal
                      <div class="time-panel">10th May</div></div>
                   <div class="text-panel">vs</div>
                   <div class="message-title">Rayo
                    </div>
              </div>
            </li>
            <!--Accordion Panel 3-->
              <li data-ej-text="Ongoing Matches">
             </li>
          </ul>
      </div>

{% endhighlight %}



![](Getting-Started_images/Getting-Started_img5.png)

