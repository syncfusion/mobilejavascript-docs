---
layout: post
title: title
description: title
platform: js
control: Dialog
documentation: ug
keywords: dialog, title
---

## Title

The Title property is used to display the title text of the Dialog box. 



{% highlight html %}

<div id="alertdlg" data-role="ejmdialog" data-ej-title="Low Battery" data-ej-mode="alert"
            data-ej-leftbuttoncaption="Dismiss" data-ej-enablemodal="true" data-ej-enableautoopen="false"
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

![](Title_images\title_img1.png)


