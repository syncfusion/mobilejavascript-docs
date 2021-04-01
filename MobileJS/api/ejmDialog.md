---
layout: post
title: ejmDialog | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmDialog
platform: Mobilejs
control: ejmDialog
documentation: API
keywords: ejmDialog, API, Essential Studio JS Dialog (Mobile)
---

# ejmDialog

The Essential JavaScript Mobile Dialog widget is an overlay positioned within the page and it displays a message such as supplementary content like images or text, and interactive content like forms. It contains a title, a content area and buttons for user interaction.

Custom Design for HTML Dialog control.

$(element).ejmDialog()

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        $("#alertdialog").ejmDialog();
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>


{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

* module:ej.mobile.scrollbar

* module:ej.mobile.scrollpanel

## Members

### allowScrolling `boolean`
{:#members:allowscrolling} 

Specifies whether to allow scrolling behavior for the contents. If this property set as true, ejmDialog will render scrollpanel automatically if the contents exceeds the content area.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->

    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-height="200px" data-ej-allowscrolling="true">
        <div>
            London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
            paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
            paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ height: "200px", allowScrolling: true });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### closeOndocumentTap `boolean`
{:#members:closeondocumenttap} 

Specifies whether the Dialog close while click on the document. If it is set as false, user need to handle Dialog close manually. 

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-closeondocumenttap="true" >
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ closeOndocumentTap: true });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### cssClass `string`
{:#members:cssclass} 

Sets the root class for Dialog theme. This cssClass API helps to use custom skinning option for Dialog control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-cssclass="customclass" >
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>

    <style>
        .customclass .e-m-dlg-content *{
            color: red;
        }
    </style>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ cssClass: "customclass" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>

    <style>
        .customclass .e-m-dlg-content *{
            color: red;
        }
    </style>



{% endhighlight %}

### enableAnimation `boolean`
{:#members:enableanimation} 

Enables or Disables animation effect on opening or closing the Dialog.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-enableanimation="false">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ enableAnimation: false });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### enableAutoOpen `boolean`
{:#members:enableautoopen} 

Specifies whether to open the Dialog on initial loading.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-enableautoopen="true">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ enableAutoOpen: true });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### enableModal `boolean`
{:#members:enablemodal} 

Specifies whether to enable modal for the Dialog or not.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-enablemodal="false">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ enableModal: false });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}


### enableNativeScrolling `boolean`
{:#members:enablenativescrolling} 

Specifies whether to enable device’s native scroll behavior when scrolling is allowed.

N> To achieve this behavior, the allowScrolling property should be set as true.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-height="200px" data-ej-allowscrolling="true" data-ej-enablenativescrolling="true">
        <div>
               London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
               paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    
        <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
            paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ height: "200px", allowScrolling: true ,enableNativeScrolling:true});
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence} 

Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-enablepersistence="true">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ enablePersistence: true });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### height `string`
{:#members:height} 

Specifies the height of Dialog content.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-height="200px">
        <div>
                 London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
                 paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
                 London : London, one of the most popular tourist destinations in the world for a reason. A cultural and historical hub, London has an excellent public transportation system that allows visitors to see all the fantastic sights without spending a ton of money on a rental car.
				     London contains four World Heritage Sites.
                 paris  : Paris, the city of lights and love - this short guide is full of ideas for how to make the most of the romanticism that oozes from every one of its beautiful corners.You couldn't possibly visit Paris without seeing the Eiffel Tower.
				     Even if you do not want to visit this world famous structure, you will see its top from all over Paris.
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ height: "200px" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### leftButtonCaption `string`
{:#members:leftbuttoncaption} 

Specifies the text of left button. For alert mode Dialog, this property specifies the alert button text.

#### Default Value

* Cancel

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-leftbuttoncaption="Done">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ leftButtonCaption: "Done" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### locale `string`
{:#members:locale} 

Specifies the localization to adopt the required language. In Dialog control title, left and right button captions are given localization support.

#### Default Value

* “en-US”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-locale="zh-CN">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        ej.mobile.Dialog.Locale['zh-CN'] = {
            title: "标题",
            leftButtonCaption: "取消",
            rightButtonCaption: "继续"
        };

        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        ej.mobile.Dialog.Locale['zh-CN'] = {
            title: "标题",
            leftButtonCaption: "取消",
            rightButtonCaption: "继续"
        };

        $("#alertdialog").ejmDialog({ locale: "zh-CN" });

        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### mode `enum`
{:#members:mode} 

Specifies the Dialog mode to render. i.e. alert mode or confirm mode. See [DialogMode](http://help.syncfusion.com/mobilejs/api/global#dialogmode)

#### Default Value

* “alert”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-mode="confirm">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ mode: "confirm" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### renderMode `enum`
{:#members:rendermode} 

Specifies the rendering mode of the control. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default Value

* auto

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-rendermode="android">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        $("#alertdialog").ejmDialog({ renderMode: "android" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>


{% endhighlight %}

### rightButtonCaption `string`
{:#members:rightbuttoncaption} 

Specifies the text of right button for confirm mode Dialog.

N> rightButtonCaption property only works for confirm mode Dialog. For confirm mode Dialog, set the property mode to “confirm”.

#### Default Value

* Continue

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-mode="confirm" data-ej-rightbuttoncaption="Ok">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ mode: "confirm", rightButtonCaption: "Ok" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### showButtons `boolean`
{:#members:showbuttons} 

Specifies whether to show the buttons in the Dialog or not.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-showbuttons="false">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        $("#alertdialog").ejmDialog({ showButtons: false });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>


{% endhighlight %}

### showHeader `boolean`
{:#members:showheader} 

Specifies whether to show the header in the Dialog or not.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-showheader="false">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        $("#alertdialog").ejmDialog({ showHeader: false });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>


{% endhighlight %}

### templateId `string`
{:#members:templateid} 

Specifies ID of the element contains template contents.

#### Default Value

* null

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-templateid="dlgcontent">
    </div>

    <script id="dlgcontent" type="text/ng-template">
        <div>
            10% of battery remaining
        </div>
    </script>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
    </div>

    <script id="dlgcontent" type="text/ng-template">
        <div>
            10% of battery remaining
        </div>
    </script>

    <script>
        $(function () {
            $("#alertdialog").ejmDialog({ templateId: "dlgcontent" });
        });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

### title `string`
{:#members:title} 

Specifies the title text.

#### Default Value

* null

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-title="Warning">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>
    <script>
        $("#alertdialog").ejmDialog({ title: "Warning" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>


{% endhighlight %}

### width `string`
{:#members:width} 

Specifies the width of Dialog content.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-width="400px">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ width: "400px" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}

## Methods

### close()
{:#methods:close} 

To close the Dialog.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-leftbuttoncaption="Close Dialog" data-ej-buttontap="close">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function close() {
            $("#alertdialog").ejmDialog("close");
        }
    </script>



{% endhighlight %}


### disableButton()
{:#methods:disablebutton} 

To disable buttons in Dialog control. It accepts a string parameter to denote which button should be disable. i.e. “left” or “right”. If no parameters passed, then this method will disable all buttons in Dialog.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog">
        <div>
            10% of battery remaining
            <input data-role="ejmbutton" type="button" data-ej-text="Disable Button" data-ej-touchend="disable" />
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function disable() {
            $("#alertdialog").ejmDialog("disableButton");
        }
    </script>



{% endhighlight %}

### enableButton()
{:#methods:enablebutton} 

To enable the disabled button in Dialog control. It accepts a string parameter to denote which button should be enable. i.e. “left” or “right”. If no parameters passed, then this method will enable all disabled buttons in Dialog.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog">
        <div>
            10% of battery remaining
            <input data-role="ejmbutton" type="button" data-ej-text="Disable Button" data-ej-touchend="disable" />
            <input data-role="ejmbutton" type="button" data-ej-text="Enable Button" data-ej-touchend="enable" />
        </div>
    </div>
    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function disable() {
            $("#alertdialog").ejmDialog("disableButton");
        }
        function enable() {
            $("#alertdialog").ejmDialog("enableButton");
        }
    </script>



{% endhighlight %}

### open()
{:#methods:open} 

To open the Dialog

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
    </script>



{% endhighlight %}


## Events

### beforeClose
{:#events:beforeclose} 

Event triggers before Dialog window get closed.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from Dialog.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
title</td><td>
string</td><td>
Returns the title of the Dialog.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-leftbuttoncaption="Close Dialog" data-ej-buttontap="closeDialog" data-ej-beforeclose="beforeClose">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function closeDialog() {
            $("#alertdialog").ejmDialog("close");
        }
        function beforeClose(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ leftButtonCaption: "Close Dialog", buttonTap: "closeDialog", beforeClose: "beforeClose" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function closeDialog() {
            $("#alertdialog").ejmDialog("close");
        }
        function beforeClose(args) {
            //handle the event
        }
    </script>



{% endhighlight %}

### buttonTap
{:#events:buttontap} 

Event triggers when tap happens on the button.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from Dialog.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
text</td><td>
Object</td><td>
Returns the text of the button.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-leftbuttoncaption="Close Dialog" data-ej-buttontap="closeDialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function closeDialog() {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ buttonTap: "closeDialog" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function closeDialog() {
            //handle the event
        }
    </script>



{% endhighlight %}

### close
{:#events:close} 

Event triggers after Dialog window get closed.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from Dialog.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
title</td><td>
string</td><td>
Returns the title of the Dialog.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-leftbuttoncaption="Close Dialog" data-ej-buttontap="closeDialog" data-ej-close="close">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function closeDialog() {
            $("#alertdialog").ejmDialog("close");
        }
        function close(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ leftButtonCaption: "Close Dialog", buttonTap: "closeDialog", close: "close" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function closeDialog() {
            $("#alertdialog").ejmDialog("close");
        }
        function close(args) {
            //handle the event
        }
    </script>



{% endhighlight %}

### open
{:#events:open} 

Event triggers after Dialog window get opened.

<table>
<tr>
<th>
<b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
argument</td><td>
Object</td><td>
Event parameters from Dialog.<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
title</td><td>
string</td><td>
Returns the title of the Dialog.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog" data-role="ejmdialog" data-ej-open="open">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function open(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input data-role="ejmbutton" type="button" data-ej-text="Open Dialog" data-ej-touchend="openAlertDialog" />
    <div id="alertdialog">
        <div>
            10% of battery remaining
        </div>
    </div>

    <script>
        $("#alertdialog").ejmDialog({ open: "open" });
        function openAlertDialog() {
            $("#alertdialog").ejmDialog("open");
        }
        function open(args) {
            //handle the event
        }
    </script>



{% endhighlight %}

