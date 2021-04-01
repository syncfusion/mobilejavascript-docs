---
layout: post
title: ejmMenu | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmMenu
platform: Mobilejs
control: ejmMenu
documentation: API
keywords: ejmMenu, API, Essential Studio JS Menu (Mobile) 
---

# ejmMenu

Mobile Menu Control provides an interface to easily navigate hierarchical data.

Custom Design for Html Menu control.

$(element).ejmMenu()


#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem" });
        });
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

### allowScrolling `Boolean`
{:#members:allowscrolling}

Specifies whether to allow scrolling behavior for the contents.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-allowscrolling=true>
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set allowScrolling on initialization.
        // To set allowScrolling API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", allowScrolling: true });
        });
    </script>


{% endhighlight %}



### cancelButton `Object`
{:#members:cancelbutton}

Specifies the cancel button of the menu control.


N>Cancel button is shown only for Actionsheet type

### cancelButton.color `String`
{:#members:cancelbutton-color}

Specifies the color of the cancel button text.

#### Default Value:

* “”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-cancelbutton-color="red">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", cancelButton: { color: "red" } });
        });
    </script>


{% endhighlight %}



### cancelButton.show `Boolean`
{:#members:cancelbutton-show}

Specifies the show or hide of the menu control.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-cancelbutton-show="false">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", cancelButton: { show: false } });
        });
    </script>


{% endhighlight %}



### cancelButton.text `String`
{:#members:cancelbutton-text}

Specifies to customize the cancel button text.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-cancelbutton-text="close">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", cancelButton: { text: "close" } });
        });
    </script>


{% endhighlight %}

### color `String`
{:#members:color}

Specifies the text color of the menu item.

#### Default Value:

* “”

#### Example

{% highlight html %}

     <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info" data-ej-color="red"></li>
            <li data-ej-text="Show in folder" data-ej-color="green"></li>
            <li data-ej-text="Delete" data-ej-color="blue"></li>
        </ul>
    </div>


{% endhighlight %}




### cssClass `String`
{:#members:cssclass}

Sets the root class for Menu theme. This cssClass API helps to use custom skinning option for Menu control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* ””

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-cssclass="customclass">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set cssClass on initialization.
        // To set cssClass API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", "cssClass": "customclass" });
        });
    </script>


{% endhighlight %}



### dataSource `data`
{:#members:datasource}

Specifies the data source for Menu rendering. In Menu, options can be given as data source of JSON array.

#### Default Value:

* []

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->    
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-datasource="window.listData" data-ej-fields-text="name"></div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->  
  <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
    </div>
    <script>
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", dataSource: window.listData, fields: { text: "name" } });
        });
    </script>


{% endhighlight %}


### enablePersistence `Boolean`
{:#members:enablepersistence}

Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.

#### Default Value:

* false

#### Example

{% highlight html %}

   <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" data-ej-enablepersistence="true" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-enablepersistence="true">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" data-ej-enablepersistence="true" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set enablePersistence on initialization.
        // To set enablePersistence API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", enablePersistence: true });
        });
    </script>


{% endhighlight %}



### enableRippleEffect `Boolean`
{:#members:enablerippleeffect}

Specifies the ripple effect for the menu control. By default in android mode its value is true and other rendermode we need to set as true.

#### Default Value:

* ej.isAndroid()?true:false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-enablerippleeffect="true">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", enableRippleEffect: true });
        });
    </script>


{% endhighlight %}



### fields
{:#members:fields}

Fields used to bind the data source and it includes following field members to make data bind easier.

### fields.color `String`
{:#members:fields-color}

Specifies the text color of menu item.

#### Default Value:

* “”.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-datasource='window.listData' data-ej-fields-color='color' data-ej-fields-text='name'>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
    </div>
    <script>
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", dataSource: window.listData, fields: { text: "name", color: "color" } });
        });
    </script>


{% endhighlight %}

### fields.href `String`
{:#members:fields-href}

Specifies the URL to navigate to when the item is clicked.

#### Default Value:

* null.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-datasource='window.listData' data-ej-fields-href='href' data-ej-fields-text='name'>
    </div>


{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
    </div>
    <script>
        $(function () {

            $("#menu").ejmMenu({ target: "menuitem", dataSource: window.listData, fields: { text: "name", href: "href" } });
        });
    </script>

{% endhighlight %}


### fields.text `String`
{:#members:fields-text}

Specifies the text to display on the menu item. 

#### Default Value:

* “”.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-datasource='window.listData' data-ej-fields-text='name'>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
    </div>
    <script>
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", dataSource: window.listData, fields: { text: "name" } });
        });
    </script>


{% endhighlight %}



### height `Int`
{:#members:height}

Specifies the height of the menu control.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-height="150">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set height on initialization.
        // To set height API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", height: 150 });
        });
    </script>


{% endhighlight %}



### href `String`
{:#members:href}

Specifies the href of the menu items.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Desktop" data-ej-href="http://js.syncfusion.com/demos/mobile/"></li>
            <li data-ej-text="Phone" data-ej-href="http://js.syncfusion.com/demos/mobile/phone"></li>
            <li data-ej-text="Home" data-ej-href="http://www.syncfusion.com"></li>
        </ul>
    </div>
    
{% endhighlight %}

### locale `String`
{:#members:locale}

Change the menu text format based on given culture.

#### Default Value:

* “en-US”

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-locale="zh-CN">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        ej.mobile.Menu.Locale['zh-CN'] = {
            title: "標題"
        };
    </script>

{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", locale: "zh-CN" });
        });
		ej.mobile.Menu.Locale['zh-CN'] = {
            title: "標題"
        };
    </script>


{% endhighlight %}



### query `ej.Query`
{:#members:query}

Specifies the query to execute with the datasource.

#### Default Value:

* null

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <script>
        var query = ej.Query().take(2);
    </script>
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-query="query" data-ej-datasource="window.listData" data-ej-fields-text="name">
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
    </div>
    <script>
        var query = ej.Query().take(2);
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", dataSource: window.listData, fields: { text: "name" }, query: query });
        });
    </script>


{% endhighlight %}



### renderMode `Enum`
{:#members:rendermode}

Specifies the rendering mode of the Menu control. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value:

* auto

#### Example

{% highlight html %}

   <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" data-ej-rendermode="auto" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-rendermode="auto">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" data-ej-rendermode="auto" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set rendermode on initialization.
        // To set renderMode API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", renderMode: ej.mobile.RenderMode.Auto });
        });
    </script>


{% endhighlight %}



### showArrow `Boolean`
{:#members:showarrow}

Specifies to show the popover menu arrow.

#### Default Value:

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-type="popover" data-ej-showarrow="true">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", showArrow: true, type: "popover" });
        });
    </script>


{% endhighlight %}



### showOn `String`
{:#members:showon}

Specifies in which action need to show the menu. See[ShowOn](http://help.syncfusion.com/mobilejs/api/global#members:showon)

#### Default Value:

* tap

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-rendermode="windows" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-rendermode="windows" data-ej-target="menuitem" data-ej-showon="taphold">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" data-ej-rendermode="windows" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set showOn on initialization.
        // To set showOn API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", showOn: "taphold", renderMode: "windows" });
        });
    </script>


{% endhighlight %}






### showTitle `Boolean`
{:#members:showtitle}

Specifies to show the action sheet and popover menu title.

#### Default Value:

* true

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-showtitle="false">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", showTitle: false });
        });
    </script>


{% endhighlight %}



### target `String`
{:#members:target}

Specifies the target element of the menu control.

#### Default Value:

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set target element ID on initialization.
        // To set target element ID value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem" });
        });
    </script>


{% endhighlight %}



### templateId `String`
{:#members:templateid}

Specifies ID of the element contains template contents.

#### Default Value:

* null

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-templateid="menuTemplate"></div>
    <div id="menuTemplate">
        <li>Get info</li>
        <li>Show in folder</li>
        <li>Delete</li>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu"></div>
    <div id="menuTemplate">
        <li>Get info</li>
        <li>Show in folder</li>
        <li>Delete</li>
    </div>
    <script>
        // Set templateId property on initialization.
        // To set templateId API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", templateId: "menuTemplate" });
        });
    </script>


{% endhighlight %}



### title `String`
{:#members:title}

Specifies to customize the action sheet and popover title text.

#### Default Value:

* “title”

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-title="CustomTitle">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", title: "CustomTitle"});
        });
    </script>


{% endhighlight %}



### type `Enum`
{:#members:type}

Specifies the type of the menu control. See ej.mobile.Menu.Type

#### Default Value:

* “actionsheet”.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-type="popover">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set type on initialization.
        // To set menu type API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", type: "popover" });
        });
    </script>


{% endhighlight %}



### width `Int`
{:#members:width}

Specifies the width of the menu control.

#### Default Value:

* null

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-width=200>
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Set width on initialization.
        // To set width API value
        $(function () {
            $("#menu").ejmMenu({ target: "menuitem", width: 200 });
        });
    </script>


{% endhighlight %}



## Methods

### addItem()
{:#methods:additem}

To add the menu item dynamically.

#### Example

{% highlight html %}

<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        $(function () {
            $("#menu").ejmMenu("addItem", "<li>Dynamic Item</li>");
        });
    </script>


{% endhighlight %}



### disable()
{:#methods:disable}

To disable the menu.

#### Example

{% highlight html %}

<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Disable the menu control
        $(function () {
            $("#menu").ejmMenu("disable");
        });
    </script>


{% endhighlight %}



### disableCancelbutton()
{:#methods:disablecancelbutton}

To disable the menu cancel button.

#### Example

{% highlight html %}

<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Disable the menu control
        $(function () {
            $("#menu").ejmMenu("disableCancelButton");
        });
    </script>


{% endhighlight %}





### disableItem()
{:#methods:disableitem}

To disable the item in the given index.

#### Example

{% highlight html %}

  <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Disable the given index menu item
        $(function () {
            $("#menu").ejmMenu("disableItem", "1");
        });
    </script>


{% endhighlight %}



### enable()
{:#methods:enable}

To enable the menu.

#### Example

{% highlight html %}

   <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>

    <script>
        // Enable the menu control
        $(function () {
            $("#menu").ejmMenu("enable");
        });
    </script>


{% endhighlight %}



### enableCancelbutton()
{:#methods:enablecancelbutton}

To enable the menu cancel button.

#### Example

{% highlight html %}

<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Disable the menu control
        $(function () {
            $("#menu").ejmMenu("enableCancelButton");
        });
    </script>


{% endhighlight %}



### enableItem()
{:#methods:enableitem}

To enable item in the given index.

#### Example

{% highlight html %}

    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>

    <script>
        // Enable the given index menu item
        $(function () {
            $("#menu").ejmMenu("enableItem", "1");
        });
    </script>


{% endhighlight %}



### hide()
{:#methods:hide}

To hide the menu.

#### Example

{% highlight html %}

<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>

    <script>
        // Hide the menu which is already opened
        $(function () {
            $("#menu").ejmMenu("hide");
        });
    </script>


{% endhighlight %}



### removeItem()
{:#methods:removeitem}

To remove item in the given index.

#### Example

{% highlight html %}

    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    // Create menu control
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // Remove the given index menu item
        $(function () {
            $("#menu").ejmMenu("removeItem", "1");
        });
    </script>


{% endhighlight %}



### show()
{:#methods:show}

To show the menu.

#### Example

{% highlight html %}

<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>

    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>

    <script>
        // Show/Open the menu which is in hide state.
        $(function () {
            $("#menu").ejmMenu("show");
        });
    </script>


{% endhighlight %}



## Events

### actionComplete
{:#events:actioncomplete}

Triggers when the AJAX requests complete. The request may get failed or succeed.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
  <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-actioncomplete="actionComplete" data-ej-datasource="window.listData" data-ej-fields-text="ContactName"></div>
    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
        // actionComplete event for menu
        function actionComplete(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu"></div>
    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                dataSource: window.listData,
                fields: { text: "ContactName" },
                actionComplete: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### actionFailure
{:#events:actionfailure}

Triggers when the data requested from AJAX get failed.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
  <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-actionfailure="actionFailure" data-ej-datasource="window.listData" data-ej-fields-text="ContactName"></div>
    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
        // actionFailure event for menu
        function actionFailure(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu"></div>
    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                dataSource: window.listData,
                fields: { text: "ContactName" },
                actionFailure: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### actionSuccess
{:#events:actionsuccess}

Triggers after the data requested via AJAX is successfully loaded.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
  <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-actionsuccess="actionSuccess" data-ej-datasource="window.listData" data-ej-fields-text="ContactName"></div>
    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
        // actionSuccess event for menu
        function actionSuccess(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu"></div>
    <script>
        window.listData = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Suppliers"
        });
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                dataSource: window.listData,
                fields: { text: "ContactName" },
                actionSuccess: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}







### hide
{:#events:hide}

Event triggers when the menu is hide.

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
Event parameters from menu.<table><br><tr><br><th>
<b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-hide="hide">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // hide event for menu
        function hide(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // hide event for menu
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                hide: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### load
{:#events:load}

Event triggers before the items loaded.

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
Event parameters from menu.<table><br><tr><br><th>
<b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-load="load">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // load event for menu
        function load(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // load event for menu
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                load: function (args) {
                    //handle the event                    
                }
            });
        });
    </script>


{% endhighlight %}



### loadComplete
{:#events:loadcomplete}

Event triggers after the items loaded.

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
Event parameters from menu.<table><br><tr><br><th>
<b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-loadcomplete="loadComplete">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // loadComplete event for menu
        function loadComplete(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // loadComplete event for menu
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                loadComplete: function (args) {
                    //handle the event                    
                }
            });
        });
    </script>


{% endhighlight %}



### show
{:#events:show}

Event triggers when the menu is shown.

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
Event parameters from menu.<table><br><tr><br><th>
<b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-show="show">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // show event for menu
        function show(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // show event for menu
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                show: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### touchEnd
{:#events:touchend}

Event triggers when touch end happens on the item.

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
Event parameters from menu.<table><br><tr><br><th>
<b>Name</b></th><th>
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
item</td><td>
Object</td><td>
Returns the current menu list element</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current menu list element associated text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-touchend="touchend">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>

    <script>
        // touchend event for menu
        function touchend(args) {
            //handle the event            
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>

    <script>
        // touchend event for menu
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                touchEnd: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



### touchStart
{:#events:touchstart}

Event triggers when touch start happens on the item.

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
Event parameters from menu.<table><br><tr><br><th>
<b>Name</b></th><th>
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
item</td><td>
Object</td><td>
Returns the current menu list element</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current menu list element associated text</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu" data-role="ejmmenu" data-ej-target="menuitem" data-ej-touchstart="touchstart">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // touchStart event for menu
        function touchstart(args) {
            //handle the event           
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<div>
        <input id="menuitem" type="button" data-role="ejmbutton" data-ej-text="Menu" />
    </div>
    <div id="menu">
        <ul>
            <li data-ej-text="Get info"></li>
            <li data-ej-text="Show in folder"></li>
            <li data-ej-text="Delete"></li>
        </ul>
    </div>
    <script>
        // touchStart event for menu
        $(function () {
            $("#menu").ejmMenu({
                target: "menuitem",
                touchStart: function (args) {
                    //handle the event
                }
            });
        });
    </script>


{% endhighlight %}



