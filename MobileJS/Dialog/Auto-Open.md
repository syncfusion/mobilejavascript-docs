---
layout: post
title: auto-open
description: auto open
platform: js
control: Dialog
keywords: dialog, autopen
documentation: ug
---

## Auto open

The EnableAutoOpen property is used to open the Dialog box on initial loading. The default value is false.

{% highlight html %}

<div id="alertdlg" data-role="ejmdialog" data-ej-title="Low Battery" data-ej-mode="alert"
        data-ej-leftbuttoncaption="Dismiss" data-ej-enablemodal="true" data-ej-enableautoopen="true"
        data-ej-buttontap="alertClose">
        <div>
            10% of battery remaining
        </div>
    </div>
    <div style="text-align: center">
        <input data-role="ejmbutton" data-ej-text="Click here to open dialog" type="button" data-ej-touchend="openAlertDialog" id="btn1" />
    </div>


{% endhighlight %}



{% highlight js %}

    function alertClose(args) {
            $("#alertdlg").ejmDialog("close");
        }
        function openAlertDialog(args) {
            $("#alertdlg").ejmDialog("open");
        }


{% endhighlight %}

![](Auto-Open_images\auto-open_img1.png)

