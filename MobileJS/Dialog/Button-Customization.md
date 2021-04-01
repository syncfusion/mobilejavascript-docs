---
layout: post
title: button-customization
description: button customization
platform: js
control: Dialog
keywords: dialog, button
documentation: ug
---

# Button customization

## Left button caption

The LeftButtonCaption property is used to specify the text of the Left Button. The default value is cancel.

{% highlight html %}

    <div style="text-align: center;">
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    </div>
    <div id="alertdialog" data-role="ejmdialog" data-ej-leftbuttoncaption="OK" data-ej-mode="confirm">
        <div>
            10% of battery remaining
        </div>
    </div>


{% endhighlight %}



{% highlight js %}

  function openAlertDialog(args) {
            $("#alertdialog").ejmDialog("open");
        }


{% endhighlight %}

![](Button-Customization_images\leftbuttoncaption_img1.png)


## Right button caption

The RightButtonCaption property specifies the text of the Right Button. The default value is continue.

{% highlight html %}

       <div style="text-align: center;">
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    </div>
    <div id="alertdialog" data-role="ejmdialog" data-ej-rightbuttoncaption="OK" data-ej-mode="confirm">
        <div>
            10% of battery remaining
        </div>
    </div>


{% endhighlight %}



{% highlight js %}

        function openAlertDialog(args) {
            $("#alertdialog").ejmDialog("open");
        }


{% endhighlight %}

![](Button-Customization_images\rightbuttoncaption_img1.png)


## Show buttons

The ShowButtons property is used to show the buttons in the Dialog box. The default value is true.

{% highlight html %}

       <div style="text-align: center;">
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    </div>
    <div id="alertdialog" data-role="ejmdialog" data-ej-showbuttons="false" data-ej-mode="confirm">
        <div>
            10% of battery remaining
        </div>
    </div>


{% endhighlight %}



{% highlight js %}

        function openAlertDialog(args) {
            $("#alertdialog").ejmDialog("open");
        }


{% endhighlight %}

![C:\Users\vigneshdr\Desktop\Mobile UG\Dialog\Emulator\8.png](Button-Customization_images\showbuttons_img1.png)