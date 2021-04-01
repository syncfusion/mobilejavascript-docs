---
layout: post
title: ejmNavigationBar | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmNavigationBar
platform: Mobilejs
control: ejmNavigationBar
documentation: API
keywords: ejmNavigationBar, API, Essential Studio JS NavigationBar (Mobile)
---

# ejmNavigationBar

The Essential JavaScript Mobile NavigationBar widget is a navigation element positioned at the top or bottom of the page, which consists of header, footer and toolbars. Header and footer consists of left and right buttons for page navigation, and toolbar consists of set of icons to support page actions.

Custom Design for HTML NavigationBar control.

$(element).ejmNavigationBar()

#### Example

**Navigation bar as header**

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header" });
    </script>



{% endhighlight %}



**Navigation bar as footer**

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="footer" data-role="ejmnavigationbar" data-ej-position="bottom" data-ej-title="Navigation Footer">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="footer">
    </div>

    <script>
        $("#footer").ejmNavigationBar({ position: "bottom", title: "Navigation Footer" });
    </script>



{% endhighlight %}



N> To get NavigationBar with left button or right buttons, render buttons inside the NavigationBar element as follows.

{% highlight html %}


    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header with buttons">
        <a data-ej-cssclass="e-m-navbar-left" data-role="ejmbutton" data-ej-style="header" data-ej-showborder="false" data-ej-contenttype="image" data-ej-imageclass="e-m-icon-backward" data-ej-text="Back"></a>
        <a data-ej-cssclass="e-m-navbar-right" data-role="ejmbutton" data-ej-style="header" data-ej-showborder="false" data-ej-contenttype="image" data-ej-imageclass="e-m-icon-next" data-ej-text="Next"></a>
    </div>



{% endhighlight %}



**Navigation bar as toolbar**

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({ mode: "toolbar" });
    </script>



{% endhighlight %}



#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

## Members

### android
{:#members:android}

Section for android mode specific functionalities.

N> Android specific properties works only in android mode. To achieve android specific properties, rendeMode property should be set as “android”.

### android.position `enum`
{:#members:android-position}

Specifies the position of NavigationBar in android rendering mode. i.e. top or bottom. See [NavBarPosition](http://help.syncfusion.com/mobilejs/api/global#navbarposition)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-rendermode="android" data-ej-android-position="bottom">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header", renderMode: "android", android: { position: "bottom" } });
    </script>



{% endhighlight %}



### badge
{:#members:badge}

Section for badge specific properties.

### badge.maxValue `number`
{:#members:badge-maxvalue}

Specifies maximum badge value which a navigation toolbar item can accept. If badge value is set a value greater than this maxValue, then the max value will be appeared with a plus sign.

#### Default Value

* 99

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-badge-maxvalue="82">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({ mode: "toolbar", badge: { maxValue: 82 } });
    </script>



{% endhighlight %}



### cssClass `string`
{:#members:cssclass}

Sets the root class for NavigationBar theme. This cssClass API helps to use custom skinning option for NavigationBar control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-cssclass="customclass">        
    </div>

    <style>
        .customclass .e-m-navbar-text {
            color: red !important;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header", cssClass: "customclass" });
    </script>

    <style>
        .customclass .e-m-navbar-text {
            color: red !important;
        }
    </style>



{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence}

Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-enablepersistence="true">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header", enablePersistence: true });
    </script>



{% endhighlight %}


### enableRippleEffect `boolean`
{:#members:enableripplerffect}

Specifies whether to enable ripple effect on toolbar item click or not.

#### Default Value

* ej.isAndroid() ? true : false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-enablerippleeffect="true">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({ mode: "toolbar", enableRippleEffect: true });
    </script>



{% endhighlight %}

### flat
{:#members:flat}

Section for flat mode specific functionalities. 

N> Flat specific properties works only in flat mode. To achieve flat specific properties, renderMode property should be set as “flat”.


### flat.position `enum`
{:#members:flat-position}

Specifies the position of NavigationBar in flat rendering mode. i.e. top or bottom. See [NavBarPosition](http://help.syncfusion.com/mobilejs/api/global#navbarposition)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-rendermode="flat" data-ej-flat-position="bottom">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header", renderMode: "flat", flat: { position: "bottom" } });
    </script>



{% endhighlight %}



### iconAlignment `enum`
{:#members:iconalignment}

It is used to align icons in a specific manner. In split alignment, icons will take 100% of page width and badge of icons will be appeared on right side of icons. In grouped alignment, icons will take some specific with and will render middle of the page, and the badge of icons will be appeared on top right of icons. See [NavBarIconAlignment](http://help.syncfusion.com/mobilejs/api/global#navbariconalignment)

N> This is a toolbar specific property. It works only when the mode property set as “toolbar” and icons of toolbar defined in sample.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-iconalignment="grouped">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({ mode: "toolbar", iconAlignment: "grouped"  });
    </script>



{% endhighlight %}



### ios7
{:#members:ios7}

Section for ios7 mode specific functionalities. 

N> Ios7 specific properties works only in ios7 mode. To achieve ios7 specific properties, rendeMode property should be set as “ios7”.


### ios7.position `enum`
{:#members:ios7-position}

Specifies the position of NavigationBar in ios7 rendering mode. i.e. top or bottom. See [NavBarPosition](http://help.syncfusion.com/mobilejs/api/global#navbarposition)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-rendermode="ios7" data-ej-ios7-position="bottom">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header", renderMode: "ios7", ios7: { position: "bottom" } });
    </script>



{% endhighlight %}



### isRelative `boolean`
{:#members:isrelative}

Specifies whether the NavigationBar render with relative position or not. By default the NavigationBar renders with absolute positioning (on the top of the page or bottom of the page if position “bottom”).

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div>
        <p>Header will render after this element</p>
    </div>
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-isrelative="true">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div>
        <p>Header will render after this element</p>
    </div>
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ isRelative: true, title: "Navigation Header" });
    </script>



{% endhighlight %}



### items `jsonarray`
{:#members:items}

Specifies the toolbar items in NavigationBar. Toolbar icons can be rendered using datasource instead of HTML ul li tags. 

N> This property is a toolbar specific. Toolbar items can be given as array of objects. To achieve this, mode property must be set as “toolbar”

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <script>
        window.data = [{ iconName: 'plus' }, { iconName: 'cut' }, { iconName: 'copy', badgeValue: 2 }, { iconName: 'save' }, { iconName: 'search', badgeValue: 333 }];
    </script>

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-items="window.data">
    </div>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({ mode: "toolbar", items: [{ iconName: "plus" }, { iconName: "cut" }, { iconName: "copy", badgeValue: 2 }, { iconName: "save" }, { iconName: "search", badgeValue: 333 }] });
    </script> 



{% endhighlight %}



### locale `string`
{:#members:locale}

Specifies the localization to adopt the required language.

#### Default Value

* “en-US”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-locale="zh-CN">        
    </div>

    <script>
        ej.mobile.NavigationBar.Locale['zh-CN'] = {
            title: "標題導航"
        };
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $(function () {
            $("#header").ejmNavigationBar({ locale: "zh-CN" });
        });
        ej.mobile.NavigationBar.Locale['zh-CN'] = {
            title: "標題導航"
        };
    </script>


{% endhighlight %}



### mode `enum`
{:#members:mode}

Specifies the mode of NavigationBar. If the value of this property is “toolbar”, then the NavigationBar will act as toolbar otherwise header. (Or footer if position is bottom). See [NavBarMode](http://help.syncfusion.com/mobilejs/api/global#navbarmode)

#### Default Value

* “header”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({ mode: "toolbar" });
    </script>



{% endhighlight %}



### position `enum`
{:#members:position}

Specifies the position of NavigationBar. i.e. top or bottom. See [NavBarPosition](http://help.syncfusion.com/mobilejs/api/global#navbarposition)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="footer" data-role="ejmnavigationbar" data-ej-position="bottom" data-ej-title="Navigation Footer">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="footer">
    </div>

    <script>
        $("#footer").ejmNavigationBar({ position: "bottom", title: "Navigation Footer" });
    </script>



{% endhighlight %}



### renderMode `enum`
{:#members:rendermode}

Specifies the rendering mode of the control. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-rendermode="android" data-ej-title="Navigation Header">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ renderMode: "android", title: "Navigation Header" });
    </script>



{% endhighlight %}



### templateId `string`
{:#members:templateId}

Specifies ID of the element contains template contents.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-templateid="headertemplate">        
    </div>

    <script id="headertemplate" type="text/ng-template">
        <div>
            <p>Template Header</p>
        </div>
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $(function () {
            $("#header").ejmNavigationBar({ templateID: "headertemplate" });
        });
    </script>

    <script id="headertemplate" type="text/ng-template">
        <div>
            <p>Template Header</p>
        </div>
    </script>


{% endhighlight %}



### titleAlignment `enum`
{:#members:titlealignment}

Specifies the title alignment of the NavigationBar. See [NavBarTitleAlignment](http://help.syncfusion.com/mobilejs/api/global#navbartitlealignment)

#### Default Value

* “left”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-titlealignment="center">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header", titleAlignment: "center" });
    </script>



{% endhighlight %}



### title `string`
{:#members:title}

Specifies the title of the NavigationBar. If this value is not set the header will render without title span.

N> For toolbar mode bottom positioned NavigationBar, the title will not be shown.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header" });
    </script>



{% endhighlight %}



### windows
{:#members:windows}

Section for windows mode specific functionalities. 

N> Windows specific properties works only in windows mode. To achieve windows specific properties, rendeMode property should be set as “windows”.

### windows.position `enum`
{:#members:windows-position}

Specifies the position of NavigationBar in windows rendering mode. i.e. top or bottom. See [NavBarPosition](http://help.syncfusion.com/mobilejs/api/global#navbarposition)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-rendermode="windows" data-ej-windows-position="bottom">        
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="header">
    </div>

    <script>
        $("#header").ejmNavigationBar({ title: "Navigation Header", renderMode: "windows", windows: { position: "bottom" } });
    </script>



{% endhighlight %}



## Methods

### addItem()
{:#methods:additem}

To add an item to the toolbar. This method accepts two arguments. First one is a string which denotes the item to be added. Second one is index of the new item and it is optional.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Add a new item" data-ej-touchend="add" />

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
        </ul>
    </div>

    <script>
        function add() {
            $("#toolbar").ejmNavigationBar("addItem", "<li data-ej-iconname='search' data-ej-badgevalue='333'></li>", 2);
        }
    </script>



{% endhighlight %}



### disableItem()
{:#methods:disableitem}

To disable an item in the toolbar which mentioned by index parameter.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable Item" data-ej-touchend="disable" />

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        function disable() {
            $("#toolbar").ejmNavigationBar("disableItem", 2);
        }
    </script>



{% endhighlight %}



### enableItem()
{:#methods:enableitem}

To enable an item in the toolbar which mentioned by index parameter.

N> To achieve this, the item should be disabled using disableItem method.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Disable Item" data-ej-touchend="disable" />
    <input data-role="ejmbutton" type="button" data-ej-text="Enable Item" data-ej-touchend="enable" />

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        function disable() {
            $("#toolbar").ejmNavigationBar("disableItem", 2);
        }
        function enable() {
            $("#toolbar").ejmNavigationBar("enableItem", 2);
        }
    </script>



{% endhighlight %}



### getTitle()
{:#methods:gettitle}

To get title of the NavigationBar.

#### Example

{% highlight html %}


    <div id="header" data-role="ejmnavigationbar" data-ej-title="Navigation Header" data-ej-isrelative="true">
    </div>
    <input data-role="ejmbutton" type="button" data-ej-text="Get Title" data-ej-touchend="get" />

    <script>
        function get() {
            alert("Title is " + $("#header").ejmNavigationBar("getTitle"));
        }
    </script>



{% endhighlight %}



### hide()
{:#methods:hide}

To hide the NavigationBar.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Hide Toolbar" data-ej-touchend="hide" />

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
        </ul>
    </div>

    <script>
        function hide() {
            $("#toolbar").ejmNavigationBar("hide");
        }
    </script>



{% endhighlight %}


### hideItem()
{:#methods:hideitem}

To hide an item in the toolbar which mentioned by index parameter.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Hide Item" data-ej-touchend="hide" />
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        function hide() {
            $("#toolbar").ejmNavigationBar("hideItem", 2);
        }
    </script>



{% endhighlight %}



### removeItem()
{:#methods:removeitem}

To remove an item in the toolbar which mentioned by index parameter.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Remove Item" data-ej-touchend="remove" />

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        function remove() {
            $("#toolbar").ejmNavigationBar("removeItem", 2);
        }
    </script>



{% endhighlight %}



### show()
{:#methods:show}

To show the hidden NavigationBar by hide() method.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Hide Toolbar" data-ej-touchend="hide" />
    <input data-role="ejmbutton" type="button" data-ej-text="Show Toolbar" data-ej-touchend="show" />

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
        </ul>
    </div>

    <script>
        function hide() {
            $("#toolbar").ejmNavigationBar("hide");
        }
        function show() {
            $("#toolbar").ejmNavigationBar("show");
        }
    </script>


{% endhighlight %}



### showItem()
{:#methods:showitem}

To show an item in the toolbar which mentioned by index parameter. 

N> To achieve this, the item must be hidden using hideItem method.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Hide Item" data-ej-touchend="hide" />
    <input data-role="ejmbutton" type="button" data-ej-text="Show Item" data-ej-touchend="show" />

    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        function hide() {
            $("#toolbar").ejmNavigationBar("hideItem", 2);
        }
        function show() {
            $("#toolbar").ejmNavigationBar("showItem", 2);
        }
    </script>



{% endhighlight %}




## Events

### ellipsisTouchEnd
{:#events:ellipsisetouchend}

Event triggers when touch end happens on the ellipsis icon.

N> Ellipsis icon will be shown automatically while the toolbar items excess the maximum length. The maximum length of icons for top positioned toolbar is 3 and for bottom positioned toolbar is 5.

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
Event parameters from NavigationBar.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns the ellipsis element object on which the touch end event happens.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-ellipsistouchend="end">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
            <li data-ej-iconname="more"></li>
        </ul>
    </div>

    <script>
        function end(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
            <li data-ej-iconname="more"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({
            mode: "toolbar",
            ellipsisTouchEnd: function (args) {
                //handle the event
            }
        });
    </script>	



{% endhighlight %}



### ellipsisTouchStart
{:#events:ellipsistouchstart}

Event triggers when touch start happens on the ellipsis icon.

N> Ellipsis icon will be shown automatically while the toolbar items excess the maximum length. The maximum length of icons for top positioned toolbar is 3 and for bottom positioned toolbar is 5.

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
Event parameters from NavigationBar.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns the ellipsis element object on which the touch start event happens.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-ellipsistouchstart="start">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
            <li data-ej-iconname="more"></li>
        </ul>
    </div>

    <script>
        function start(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
            <li data-ej-iconname="more"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({
            mode: "toolbar",
            ellipsisTouchStart: function (args) {
                //handle the event
            }
        });
    </script>	



{% endhighlight %}



### touchEnd
{:#events:touchend}

Event triggers when touch end happens on the toolbar items.

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
Event parameters from NavigationBar.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns the element object on which the touch end event happens.</td></tr>
<tr>
<td>
iconname</td><td>
string</td><td>
Returns the name of the item on which the touch end event happens.</td></tr>
<tr>
<td>
index</td><td>
Number</td><td>
Returns the index of the item on which the touch end event happens.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-touchstart="end">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        function end(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({
            mode: "toolbar",
            touchEnd: function (args) {
                //handle the event
            }
        });
    </script>	



{% endhighlight %}



### touchStart
{:#events:touchstart}

Event triggers when touch start happens on the toolbar items.

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
Event parameters from NavigationBar.<table><br><tr><br><th><b>Name</b></th><th>
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
object</td><td>
Returns the model value of the control.</td></tr>
<tr>
<td>
element</td><td>
object</td><td>
Returns the element object on which the touch start event happens.</td></tr>
<tr>
<td>
iconname</td><td>
string</td><td>
Returns the name of the item on which the touch start event happens.</td></tr>
<tr>
<td>
index</td><td>
Number</td><td>
Returns the index of the item on which the touch start event happens.</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="toolbar" data-role="ejmnavigationbar" data-ej-mode="toolbar" data-ej-touchstart="start">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        function start(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="toolbar">
        <ul>
            <li data-ej-iconname="plus"></li>
            <li data-ej-iconname="cut"></li>
            <li data-ej-iconname="copy" data-ej-badgevalue="2"></li>
            <li data-ej-iconname="save"></li>
            <li data-ej-iconname="search" data-ej-badgevalue="333"></li>
        </ul>
    </div>

    <script>
        $("#toolbar").ejmNavigationBar({
            mode: "toolbar",
            touchStart: function (args) {
                //handle the event
            }
        });
    </script>	



{% endhighlight %}




