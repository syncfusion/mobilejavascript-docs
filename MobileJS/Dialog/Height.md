---
layout: post
title: height
description: height
platform: js
control: Dialog
documentation: ug
keywords: dialog, height
---

## Height

 The Height property specifies the height of the Dialog.

{% highlight html %}

    <div style="text-align: center;">
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    </div>
    <div id="alertdialog" data-role="ejmdialog" data-ej-height="200px" data-ej-buttontap="alertClose">
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

![](Height_images\height_img1.png)

