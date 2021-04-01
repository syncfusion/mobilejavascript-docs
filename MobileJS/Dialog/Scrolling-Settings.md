---
layout: post
title: scrolling-settings
description: scrolling settings
platform: js
control: Dialog
documentation: ug
keywords: dialog, scrolling
---

## Scrolling Settings

## AllowScrolling

The AllowScrolling property is used to enable scrollingbehavior for the Dialog content. The default value is true.

{% highlight html %}

    <div style="text-align: center;">
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    </div>
    <div id="alertdialog" data-role="ejmdialog" data-ej-height="200px" data-ej-buttontap="alertClose" data-ej-allowscrolling="true">
        <div>
            The Essential JavaScript Mobile Dialog widget is an overlay positioned and it displays a message such as supplementary content like images or text, and interactive content like forms. It contains a title and a content area.Modal Dialog support: Displays the content in a modal Dialog, disabling interaction with other items on the page.Auto open: By default, the Dialog is in a disable state. It enables or disables the Dialog state.
        </div>
    </div>


{% endhighlight %}



{% highlight js %}

        function alertClose(args) {
            $("#alertdialog").ejmDialog("close");
        }
        function openAlertDialog(args) {
            $("#alertdialog").ejmDialog("open");
        }


{% endhighlight %}

![](Scroll-Settings_images\allowscrolling_img1.png)


## EnableNativeScrolling

The EnableNativeScrolling property is used to enable native (built-in browser) scrolling functionality of the devices when scrolling is allowed. The default value is false.

{% highlight html %}

    <div style="text-align: center;">
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    </div>
    <div id="alertdialog" data-role="ejmdialog" data-ej-height="200px" data-ej-buttontap="alertClose" data-ej-enablenativescrolling="true" data-ej-allowscrolling="true">
        <div>
            The Essential JavaScript Mobile Dialog widget is an overlay positioned and it displays a message such as supplementary content like images or text, and interactive content like forms. It contains a title and a content area.Modal Dialog support: Displays the content in a modal Dialog, disabling interaction with other items on the page.Auto open: By default, the Dialog is in a disable state. It enables or disables the Dialog state.
        </div>
    </div>


{% endhighlight %}



{% highlight js %}

        function alertClose(args) {
            $("#alertdialog").ejmDialog("close");
        }
        function openAlertDialog(args) {
            $("#alertdialog").ejmDialog("open");
        }


{% endhighlight %}
