---
layout: post
title: ejmDropDownList | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmDropDownList
platform: Mobilejs
control: ejmDropDownList
documentation: API
keywords: ejmDropDownList, API, Essential Studio JS DropDownList (Mobile)
---

# ejmDropDownList

The Essential JavaScript Mobile DropDownList widget is a text box control that provides a list of options on focus and allows you to pick one option.

Custom Design for HTML DropDownList control.

$(element).ejmDropDownList()

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle" });
    </script>



{% endhighlight %}



#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

* module:ej.mobile.listview

* module:ej.mobile.scrollpanel

* module:ej.mobile.scrollbar

## Members

### allowVirtualScrolling `boolean`
{:#members:allowvirtualscrolling}

The Virtual Scrolling feature is used to display a large amount of records in the DropDownList, that is when scroll end happens, an AJAX request is sent to fetch some amount of data from the server dynamically. To achieve this scenario with DropDownList, set the allowVirtualScrolling to true. You can set the itemsCount property that represents the number of items to be fetched from the server on every AJAX request. 

N> To achieve virtual scrolling, dataSource, fields.text and itemsCount properties should be set properly.

#### Default Value

* false



#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dd_virtualscroll" data-role="ejmdropdownlist" data-ej-datasource="window.datasrc" data-ej-fields-text="ContactName" data-ej-allowvirtualscrolling="true" data-ej-itemscount="10" />

    <script type="text/javascript">
        window.datasrc = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Customers"
        });
    </script> 



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="virtualscroll" />

    <script type="text/javascript">
        window.datasrc = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Customers"
        });
        $("#virtualscroll").ejmDropDownList({ dataSource: window.datasrc, fields: { text: "ContactName" }, itemsCount: 10, allowVirtualScrolling: true });
    </script> 



{% endhighlight %}



### cssClass `string`
{:#members:cssclass}

Sets the root class for DropDownList. This cssClass API helps to use custom skinning option for DropDownList control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-cssclass="customclass" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <style>
        .customclass .e-m-dropdownlist {
            color: red !important;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", cssClass: "customclass" });
    </script>

    <style>
        .customclass .e-m-dropdownlist {
            color: red !important;
        }
    </style>



{% endhighlight %}



### dataSource `jsonarray`
{:#members:datasource}

Specifies the data source for DropDownList rendering. In DropDownList, options can be given as data source of JSON array.

#### Default Value:

* []

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData" data-ej-fields-text="name" />

    <script>
        window.listData = [{ name: "Australia" },
                           { name: "Brazil" },
                           { name: "China" },
                           { name: "India" },
                           { name: "Spain" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dd_default" />
    <script>
        window.listData = [{ name: "Australia" },
                           { name: "Brazil" },
                           { name: "China" },
                           { name: "India" },
                           { name: "Spain" }];
    </script>

    <script>
        $("#dd_default").ejmDropDownList({ dataSource: window.listData, fields: { text: "name" } });
    </script>


{% endhighlight %}



### delimiterChar `string`
{:#members:delimiterchar}

Specifies the separator character for multi selection mode which separates two items. 

N> This property works only for multi selection mode, hence the property enableMultiSelect should be set as true.

#### Default Value

* ”,”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-delimiterchar="/" data-ej-enablemultiselect="true" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", delimiterChar: "/", enableMultiSelect: true });
    </script>



{% endhighlight %}



### enabled `boolean`
{:#members:enabled}

Specifies whether to enable or disable the DropDownList control.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-enabled="false" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", enabled: false });
    </script>



{% endhighlight %}



### enableMultiSelect `boolean`
{:#members:enablemultiselect}

Specifies multi select DropDownList. You can select multiple options by enabling this property.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-enablemultiselect="true" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", enableMultiSelect: true });
    </script>



{% endhighlight %}



### enablePersisitence `boolean`
{:#members:enablepersisitence}

Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-enablepersistence="true" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", enablePersistence: true });
    </script>



{% endhighlight %}



### fields

Fields used to bind the data source and it includes following field members to make data bind easier.

### fields.checkBy `boolean`
{:#members:fields-checkby}

Maps the check status for each option in DropDownList initially. This is an optional property used only for multi selection DropDownList.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData" data-ej-enablemultiselect="true" data-ej-fields-text="name" data-ej-fields-checkby="check" />

    <script>
        window.listData = [{ name: "Australia", check: true },
                           { name: "Brazil" },
                           { name: "China", check: true },
                           { name: "India" },
                           { name: "Spain" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dd_default" />
    <script>
        window.listData = [{ name: "Australia", check: true },
                           { name: "Brazil" },
                           { name: "China", check: true },
                           { name: "India" },
                           { name: "Spain" }];
    </script>

    <script>
        $("#dd_default").ejmDropDownList({ dataSource: window.listData, enableMultiSelect: true, fields: { text: "name", checkBy: "check" } });
    </script>



{% endhighlight %}



### fields.groupBy `string`
{:#members:fields-groupby}

Maps the group name in which each option belongs to in DropDownList. This is an optional property used only for grouped DropDownList.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData" data-ej-fields-text="name" data-ej-fields-groupby="group" />

    <script>
        window.listData = [{ name: "Abarth", group: "Car" },
                         { name: "Audi", group: "Car" },
                         { name: "Texas", group: "Bike" },
                         { name: "Bajaj", group: "Bike" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dd_default" />
    <script>
        window.listData = [{ name: "Abarth", group: "Car" },
                         { name: "Audi", group: "Car" },
                         { name: "Texas", group: "Bike" },
                         { name: "Bajaj", group: "Bike" }];
    </script>

    <script>
        $("#dd_default").ejmDropDownList({ dataSource: window.listData, fields: { text: "name", groupBy: "group" } });
    </script>



{% endhighlight %}



### fields.image `string`
{:#members:fields-image}

Maps image field from the data source. This is a required property while rendering the DropDownList from data source. 

N> Since field mapping depends on data source, the dataSource property must be set with a JSON data.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData" data-ej-fields-text="name" data-ej-fields-image="image" />

    <script>
        window.listData = [{ name: "Australia", image: "Australia.png" },
                           { name: "Brazil", image: "Brazil.png" },
                           { name: "China", image: "china.png" },
                           { name: "India", image: "India.png" },
                           { name: "Spain", image: "Spain.png" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dd_default" />
    <script>
        window.listData = [{ name: "Australia", image: "Australia.png" },
                           { name: "Brazil", image: "Brazil.png" },
                           { name: "China", image: "china.png" },
                           { name: "India", image: "India.png" },
                           { name: "Spain", image: "Spain.png" }];
    </script>

    <script>
        $("#dd_default").ejmDropDownList({ dataSource: window.listData, fields: { text: "name", image: "image" } });
    </script>



{% endhighlight %}


### fields.text `string`
{:#members:fields-text}

Maps text field from the data source. This is a required property while rendering the DropDownList from data source. 

N> Since field mapping depends on data source, the dataSource property must be set with a JSON data.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData" data-ej-fields-text="name" />

    <script>
        window.listData = [{ name: "Australia" },
                           { name: "Brazil" },
                           { name: "China" },
                           { name: "India" },
                           { name: "Spain" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dd_default" />
    <script>
        window.listData = [{ name: "Australia" },
                           { name: "Brazil" },
                           { name: "China" },
                           { name: "India" },
                           { name: "Spain" }];
    </script>

    <script>
        $("#dd_default").ejmDropDownList({ dataSource: window.listData, fields: { text: "name" } });
    </script>



{% endhighlight %}



### fields.value `string`
{:#members:fields-value}

Maps the value for each option from the data source. This is an optional property. 

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dd_grouping" data-role="ejmdropdownlist" data-ej-datasource="window.listData" data-ej-fields-text="name" data-ej-fields-value="name" />

    <script>
        window.listData = [{ name: "Australia" },
                           { name: "Brazil" },
                           { name: "China" },
                           { name: "India" },
                           { name: "Spain" }];
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dd_default" />
    <script>
        window.listData = [{ name: "Australia" },
                           { name: "Brazil" },
                           { name: "China" },
                           { name: "India" },
                           { name: "Spain" }];
    </script>

    <script>
        $("#dd_default").ejmDropDownList({ dataSource: window.listData, fields: { text: "name", value: "name" } });
    </script>



{% endhighlight %}



### itemsCount `number`
{:#members:itemscount}

Specifies how many items need to render initially from remote data source. You can set the items count using itemsCount property that represents the number of items to be fetched from the server on every AJAX request in virtual scrolling feature.

N> This property works based on remote data source, hence the dataSource and fields.text properties should be set properly while rendering.

#### Default Value

* 0

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="query" data-role="ejmdropdownlist" data-ej-datasource="window.datasrc" data-ej-fields-text="ContactName" data-ej-itemscount="10"/>

    <script type="text/javascript">
        window.datasrc = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Customers"
        });
    </script> 



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="query" />

    <script type="text/javascript">
        window.datasrc = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Customers"
        });
        $("#query").ejmDropDownList({ dataSource: window.datasrc, fields: { text: "ContactName" }, itemsCount: 10 });
    </script> 



{% endhighlight %}



### locale `string`
{:#members:locale}

Specifies the localization to adopt the required language. In DropDownList control, localization support given for watermarkText property.

#### Default Value

* “en-US”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-locale="zh-CN" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        ej.mobile.DropDownList.Locale['zh-CN'] = {
            watermarkText: "選擇搜索引擎"
        };
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        ej.mobile.DropDownList.Locale['zh-CN'] = {
            watermarkText: "選擇搜索引擎"
        };

        $("#dd_default").ejmDropDownList({ targetId: "targetEle", locale: "zh-CN" });
    </script>



{% endhighlight %}



### popupHeight `string`
{:#members:popupheight}

Specifies the height of the options list.

#### Default Value

* ”164px”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-popupheight="205px" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
        <li data-ej-text="Aol Search"></li>
        <li data-ej-text="Wow"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
        <li data-ej-text="Aol Search"></li>
        <li data-ej-text="Wow"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", popupHeight: "205px" });
    </script>



{% endhighlight %}



### popupWidth `string`
{:#members:popupwidth}

Specifies the width of the options list.

#### Default Value

* ”auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-popupwidth="50%" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", popupWidth: "50%" });
    </script>



{% endhighlight %}



### query `string`
{:#members:query}

This property used to filter data from remote data source.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dropdown" data-role="ejmdropdownlist" data-ej-datasource="window.data" data-ej-query="ej.Query().from('Orders').select('ShipCity').take(20)" data-ej-fields-text="ShipCity" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
        });
    </script> 



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dropdown" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
        });
        $("#dropdown").ejmDropDownList({ dataSource: window.data, fields: { text: "ShipCity" }, query: "ej.Query().from('Orders').select('ShipCity').take(20)" });
    </script>



{% endhighlight %}



### readOnly `boolean`
{:#members:readonly}

Specifies whether the DropDownList to be rendered without interaction. If this set as true, you can’t focus the DropDownList textbox. 

#### Default Value

* false

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-readonly="true" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", readOnly: true });
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
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-rendermode="android" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", renderMode: "android" });
    </script>



{% endhighlight %}



### selectedItemIndex `number`
{:#members:selecteditemindex}

Specifies the Item Index which is selected initially. If the value -1 means, no item selected initially.

#### Default Value

* -1

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-selecteditemindex="1" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", selectedItemIndex: 1 });
    </script>



{% endhighlight %}



### targetId `string`
{:#members:targetid}

Specifies the target element which consists the list of options to render DropDownList. Unless data source type rendering, DropDownList needs this property must.

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle" });
    </script>



{% endhighlight %}



### templateId `string`
{:#members:templateid}

Specifies ID of the element that contains template contents.

N> For DropDownList template rendering, jsrender.js file reference needed.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="template" data-role="ejmdropdownlist" data-ej-templateid="templatecontent" data-ej-datasource="window.listData" data-ej-fields-text="Name" />

    <script id="templatecontent" type="text/x-jsrender">
        <div class="contentdiv">
            <span class="name">{{>Name}}</span> <span class="designation">{{>Designation}}</span>
        </div>
    </script>

    <script type="text/javascript">
        window.listData =
        [{ "Name": "Brooke", "Designation": "HR Assistant" },
        { "Name": "Claire", "Designation": "HR Manager" },
        { "Name": "Erik", "Designation": "Training Specialist" },
        { "Name": "Grace", "Designation": "Development Manager" },
        { "Name": "Jacob", "Designation": "Recruitment Manager" }];
    </script> 

    <style>
        .name {
            margin-left: 15px;
        }

        .designation {
            font-size: 13px;
            float: right;
            margin-right: 15px;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="template"/>

    <script id="templatecontent" type="text/x-jsrender">
        <div class="contentdiv">
            <span class="name">{{>Name}}</span> <span class="designation">{{>Designation}}</span>
        </div>
    </script>

    <script type="text/javascript">
        window.listData =
        [{ "Name": "Brooke", "Designation": "HR Assistant" },
        { "Name": "Claire", "Designation": "HR Manager" },
        { "Name": "Erik", "Designation": "Training Specialist" },
        { "Name": "Grace", "Designation": "Development Manager" },
        { "Name": "Jacob", "Designation": "Recruitment Manager" }];

        $("#template").ejmDropDownList({ templateId: "templatecontent", dataSource: window.listData, fields: { text: "Name" } });

    </script> 

    <style>
        .name {
            margin-left: 15px;
        }

        .designation {
            font-size: 13px;
            float: right;
            margin-right: 15px;
        }
    </style>



{% endhighlight %}



### watermarkText `string`
{:#members:watermarktext}

Specifies the DropDownList watermark text that to be shown on DropDownList textbox when it is empty

#### Default Value

* null

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-watermarktext="Select a search engine" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", watermarkText: "Select a search engine" });
    </script>



{% endhighlight %}



## Methods


### getSelectedItemValue()
{:#methods:getselecteditemvalue}

To get the values of currently selected item/items in DropDownList.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Get Value" data-ej-touchend="getvalue" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function getvalue() {
            var str = $("#dd_default").ejmDropDownList("getSelectedItemValue");
            alert("Currently selected value is: " + str);
        }
    </script>



{% endhighlight %}



### getValue()
{:#methods:getvalue}

To get the current selected values from DropDownList textbox.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Get Value" data-ej-touchend="getvalue" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function getvalue() {
            var str = $("#dd_default").ejmDropDownList("getValue");
            alert("Currently selected value is: " + str);
        }
    </script>



{% endhighlight %}



### hidePopup()
{:#methods:hidepopup}

To hide options list pop up.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Hide options" data-ej-touchend="hide" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function hide() {
            $("#dd_default").ejmDropDownList("hidePopup");
        }
    </script>



{% endhighlight %}



### selectItemByIndex()
{:#methods:selectitembyindex}

To select an option by its index.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Select 2nd indexed option" data-ej-touchend="select" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function select() {
            $("#dd_default").ejmDropDownList("selectItemByIndex", 2);
        }
    </script>



{% endhighlight %}



### selectItemByIndices()
{:#methods:selectitembyindices}

To select multiple option by its index array. This method works only for multi selection DropDownList. So enableMultiSelect property should be set as true.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Select 2nd, 3rd indexed options" data-ej-touchend="select" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-enablemultiselect="true" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function select() {
            $("#dd_default").ejmDropDownList("selectItemByIndices", [2, 3]);
        }
    </script>



{% endhighlight %}



### showPopup()
{:#methods:showpopup}

To show options list pop up.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Show options" data-ej-touchend="show" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function show() {
            $("#dd_default").ejmDropDownList("showPopup");
        }
    </script>



{% endhighlight %}



### unselectItemByIndex()
{:#methods:unselectitembyindex}

To unselect an option by its index. This method works only for multi selection DropDownList. So enableMultiSelect property should be set as true.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Select 2nd indexed option" data-ej-touchend="select" />
    <input data-role="ejmbutton" type="button" data-ej-text="Unselect 2nd indexed option" data-ej-touchend="unselect" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-enablemultiselect="true" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function select() {
            $("#dd_default").ejmDropDownList("selectItemByIndex", 2);
        }
        function unselect() {
            $("#dd_default").ejmDropDownList("unselectItemByIndex", 2);
        }
    </script>



{% endhighlight %}



### unselectItemByIndices()
{:#methods:unselectitembyindices}

To unselect multiple option by its index array. This method works only for multi selection DropDownList. So enableMultiSelect property should be set as true.

#### Example

{% highlight html %}


    <input data-role="ejmbutton" type="button" data-ej-text="Select 2nd, 3rd indexed options" data-ej-touchend="select" />
    <input data-role="ejmbutton" type="button" data-ej-text="Unselect 2nd, 3rd indexed options" data-ej-touchend="unselect" />
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-enablemultiselect="true" data-ej-targetid="targetEle" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function select() {
            $("#dd_default").ejmDropDownList("selectItemByIndices", [2, 3]);
        }
        function unselect() {
            $("#dd_default").ejmDropDownList("unselectItemByIndices", [2, 3]);
        }
    </script>



{% endhighlight %}


## Events

### actionComplete
{:#events:actioncomplete}

Event triggers when Ajax request succeeded and completed the processing of remote data source.

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
Event parameters from DropDownList.<table><br><tr><br><th><b>Name</b></th><th>
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
count</td><td>
number</td><td>
Returns number of times trying to fetch the data</td></tr>
<tr>
<td>
query</td><td>
object</td><td>
Returns the query for data retrieval</td></tr>
<tr>
<td>
request</td><td>
object</td><td>
Returns the query for data retrieval from the Database</td></tr>
<tr>
<td>
result</td><td>
array</td><td>
Returns the number of items fetched from remote data</td></tr>
<tr>
<td>
xhr</td><td>
object</td><td>
Returns the requested data</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dropdown" data-role="ejmdropdownlist" data-ej-datasource="window.data" data-ej-query="ej.Query().from('Orders').select('ShipCity').take(20)" data-ej-fields-text="ShipCity" data-ej-actioncomplete="complete" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
        });

        function complete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}





{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dropdown" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
        });
        $("#dropdown").ejmDropDownList({ dataSource: window.data, fields: { text: "ShipCity" }, query: "ej.Query().from('Orders').select('ShipCity').take(20)", actionComplete: "complete" });

        function complete(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### actionFailure
{:#events:actionfailure}

Event triggers when Ajax request failed for remote binding data source.

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
Event parameters from DropDownList.<table><br><tr><br><th><b>Name</b></th><th>
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
error</td><td>
object</td><td>
Returns object which contains AJAX error information</td></tr>
<tr>
<td>
query</td><td>
object</td><td>
Returns the query for data retrieval</td></tr>
</table>


</td></tr>
</table>


#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dropdown" data-role="ejmdropdownlist" data-ej-datasource="window.data" data-ej-query="ej.Query().from('Orders').select('ShipCity').take(20)" data-ej-fields-text="ShipCity" data-ej-actionfailure="error" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/North.svc"
        });

        function error(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dropdown" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/North.svc"
        });
        $("#dropdown").ejmDropDownList({ dataSource: window.data, fields: { text: "ShipCity" }, query: "ej.Query().from('Orders').select('ShipCity').take(20)", actionFailure: "error" });
        function error(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### actionSuccess
{:#events:actionsuccess}

Event triggers when Ajax request succeeded for remote binding data source.

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
Event parameters from DropDownList.<table><br><tr><br><th><b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input type="text" id="dropdown" data-role="ejmdropdownlist" data-ej-datasource="window.data" data-ej-query="ej.Query().from('Orders').select('ShipCity').take(20)" data-ej-fields-text="ShipCity" data-ej-actionsuccess="success" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
        });

        function success(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input type="text" id="dropdown" />

    <script type="text/javascript">
        window.data = ej.DataManager({
            url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
        });
        $("#dropdown").ejmDropDownList({ dataSource: window.data, fields: { text: "ShipCity" }, query: "ej.Query().from('Orders').select('ShipCity').take(20)", actionSuccess: "success" });

        function success(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### change
{:#events:change}

Event triggers when newly selected option updated to the DropDownList textbox.

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
Event parameters from DropDownList.<table><br><tr><br><th><b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-change="change"/>

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function change(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", change: "change"  });
        function change(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



### focusIn
{:#events:focusin}

Event triggers when focus in happens on the DropDownList textbox.

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
Event parameters from DropDownList.<table><br><tr><br><th><b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-focusin="focusin"/>

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function focusin(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle" , focusIn: "focusin"  });
        function focusin(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



### focusOut
{:#events:focusout}

Event triggers when focus out happens on the DropDownList textbox.

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
Event parameters from DropDownList.<table><br><tr><br><th><b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-focusout="focusout"/>

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function focusout(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle" , focusOut: "focusout"  });
        function focusout(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



### select
{:#events:select}

Event triggers when an option selected from the options list but not updated to the DropDownList textbox.

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
Event parameters from DropDownList.<table><br><tr><br><th><b>Name</b></th><th>
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
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <input id="dd_default" data-role="ejmdropdownlist" data-ej-targetid="targetEle" data-ej-select="select"/>

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        function select(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <input id="dd_default" />

    <ul id="targetEle">
        <li data-ej-text="Google"></li>
        <li data-ej-text="Bing"></li>
        <li data-ej-text="Yahoo"></li>
        <li data-ej-text="Ask"></li>
    </ul>

    <script>
        $("#dd_default").ejmDropDownList({ targetId: "targetEle", select: "select"  });
        function select(args) {
            //handle the event
        }
    </script>	



{% endhighlight %}



