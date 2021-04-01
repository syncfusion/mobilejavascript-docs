---
layout: post
title: mode
description: mode
platform: js
control: Dialog
documentation: ug
keywords: dialog, mode
---

## Mode

The mode property specifies the different types of dialog modes. The possible values are, 

1. alert 

2. confirm.

3. custom.



{% highlight html %}

    <div style="text-align: center;">
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    </div>
    <div id="alertdialog" data-role="ejmdialog" data-ej-mode="confirm">
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

![](Mode_images\mode_img1.png)

