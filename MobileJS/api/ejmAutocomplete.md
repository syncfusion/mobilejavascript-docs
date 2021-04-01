---
layout: post
title: ejmAutocomplete | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmAutocomplete
platform: Mobilejs
control: ejmAutocomplete
documentation: API
keywords: ejmAutocomplete, API, Essential Studio JS AutoComplete (Mobile) 
---

# ejmAutocomplete
The Essential JavaScript Mobile AutoComplete widget is a text box control that provides a list of suggestions based on a user’s query.  

Custom Design for HTML AutoComplete control.

$(element).ejmAutocomplete()

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />    


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        // Create autocomplete
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.mobile.listview

* module:ej.mobile.scrollpanel

* module:ej.data

* module:ej.touch



## Members

### allowSorting `Boolean`
{:#members:allowsorting}

Specifies the whether allowSorting to be allowed or not in suggestion list on initialization

#### Default Value: 

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-allowsorting=true data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the allowSorting API value
        $("#autocomplete").ejmAutocomplete({ allowSorting: true, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### caseSensitiveSearch `Boolean`
{:#members:casesensitivesearch}

Specifies whether to search key is case sensitive or not on initialization.

#### Default Value: 

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-casesensitivesearch=true data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the caseSensitiveSearch API value
        $("#autocomplete").ejmAutocomplete({ caseSensitiveSearch: true, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}



### cssClass `String`
{:#members:cssclass}

Sets the root class for AutoComplete theme. This cssClass API helps to use custom skinning option for AutoComplete control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value: 

* ””

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-cssclass="customclass" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the cssClass API value
        $("#autocomplete").ejmAutocomplete({ cssClass: "customclass", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### dataSource `data`
{:#members:datasource}

Specifies the data source for AutoComplete rendering. In AutoComplete , options can be given as data source of JSON array.

#### Default Value: 

* []

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />    


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        // Create autocomplete
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}



### delimiterChar `String`
{:#members:delimiterchar}

Specifies the delimiterChar string for Multivalue mode that separates two items.

#### Default Value: 

* ”,”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-enablemultiselect="true" data-ej-delimiterchar="-" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        // Create autocomplete
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", enableMultiSelect: true, delimiterChar: "-", fields: { text: "name" } });
    </script>


{% endhighlight %}

### emptyResultText `String`
{:#members:emptyresulttext}

Specifies the text that to be displayed while there is no suggestion for AutoComplete search key

#### Default Value: 

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-emptyresulttext="No suggestions" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the emptyResultText API value
        $("#autocomplete").ejmAutocomplete({ emptyResultText: "No suggestions", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### enableAutoFill `Boolean`
{:#members:enableautofill}

Specifies whether to auto fill option by which we can select and show up the first search result in textbox on initialization.

#### Default Value: 

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-enableautofill=true data-ej-datasource="window.datasrc" data-ej-fields-text="name" />



{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enableAutoFill API value
        $("#autocomplete").ejmAutocomplete({ enableAutoFill: true, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### enabled `Boolean`
{:#members:enabled}

Specifies whether to enable the autoComplete on initialization.

#### Default Value: 

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-enabled=false data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enabled API value
        $("#autocomplete").ejmAutocomplete({ enabled: false, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}



### enableDistinct `Boolean`
{:#members:enabledistinct}

Specifies whether the duplicate results to be shown or not in search results

#### Default Value: 

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-enabledistinct=true data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enableDistinct API value
        $("#autocomplete").ejmAutocomplete({ enableDistinct: false, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### enableMultiSelect `Boolean`
{:#members:enablemultiselect}

Specifies whether to accept multiple values or not.

#### Default Value: 

* false

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-enablemultiselect=true data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enableMultiSelect API value
        $("#autocomplete").ejmAutocomplete({ enableMultiSelect: true, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}

### enablePersistence `Boolean`
{:#members:enablepersistence}

Current model value to browser cookies for state maintains. While refresh the Autocomplete control page retains the model value apply from browser cookies.

#### Default Value: 

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-enablepersistence=false data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enablePersistence API value
        $("#autocomplete").ejmAutocomplete({ enablePersistence: false, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### fields
{:#members:fields}

Fields used to bind the data source and it includes following field members to make data bind easier.


### fields.image `String`
{:#members:fields-image}

Specifies the name of the field from the data source that contains image URL values.

#### Default Value: 

* null.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-image="image" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enablePersistence API value
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name", image: "image" } });
    </script>


{% endhighlight %}

### fields.key `String`
{:#members:fields-key}

Specifies the field name which contains unique key values for the list items.

#### Default Value: 

* null.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-key="key" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enablePersistence API value
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name", key: "key" } });
    </script>


{% endhighlight %}


### fields.text `String`
{:#members:fields-text}

Specifies the name of the field from the data source to bind to the Text property of an AutoComplete item.

#### Default Value: 

* null.

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the enablePersistence API value
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### filterType `Enum`
{:#members:filtertype}

Specifies the type of the filter by which the filtering occurs. See[FilterType](http://help.syncfusion.com/mobilejs/api/global#members:filtertype)

#### Default Value: 

* startswith

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-filtertype="contains" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the filterType API value
        $("#autocomplete").ejmAutocomplete({ filterType: "contains", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}



### itemsCount `Number`
{:#members:itemscount}

Specifies the number of items shown in the suggestion list.

#### Default Value: 

* 0

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-itemscount=5 data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        //To set the itemsCount API value
        $("#autocomplete").ejmAutocomplete({ itemsCount: 5, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### locale `String`
{:#members:locale}

Change the AutoComplete text format based on given culture.

#### Default Value: 

* “en-US”

#### Example

{% highlight html %}

    <!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-locale="en-US" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the mode API value
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" }, locale: "en-US" });
    </script>


{% endhighlight %}


### minCharacter `Number`
{:#members:mincharacter}

Specifies the minimum search key length, which only AutoComplete queries from the datasource.

#### Default Value: 

* 1

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-mincharacter=2 data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        //To set the minCharacter API value
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" }, minCharacter: 2 });
    </script>


{% endhighlight %}



### mode `Enum`
{:#members:mode}

Specifies the AutoComplete mode. See[Mode](http://help.syncfusion.com/mobilejs/api/global#members:mode)                                            

#### Default Value: 

* default

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-mode="search" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        //To set the mode API value
        $("#autocomplete").ejmAutocomplete({ mode: "search", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### popupHeight `String`
{:#members:popupheight}

Specifies the AutoComplete popup height.

#### Default Value: 

* “164px”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-popupheight="100px" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the mode API value
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" }, popupHeight: "100px" });
    </script>


{% endhighlight %}



### popupWidth `String`
{:#members:popupwidth}

Specifies the AutoComplete popup width.

#### Default Value: 

* “auto”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
   <input id="autocomplete" data-role="ejmautocomplete" data-ej-popupwidth="500px" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the mode API value
        $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" }, popupWidth: "500px" });
    </script>


{% endhighlight %}



### renderMode `Enum`
{:#members:rendermode}

Changes the rendering mode of the autocomplete. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value: 

* auto

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-rendermode="auto" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the renderMode API value
        $("#autocomplete").ejmAutocomplete({ renderMode: ej.mobile.RenderMode.Auto, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}

### showEmptyResultText `Boolean`
{:#members:showemptyresulttext}

Specifies the search result to be shown or not while there is no suggestion for AutoComplete search key

#### Default Value: 

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-showemptyresulttext=false data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the showEmptyResultText API value
        $("#autocomplete").ejmAutocomplete({ showEmptyResultText: false, dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}




### sortOrder `Enum`
{:#members:sortorder}

Specifies the suggestion list sorting order. See[SortOrder](http://help.syncfusion.com/mobilejs/api/global#members:sortorder)

#### Default Value: 

* ascending

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-sortorder="descending" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the sortOrder API value
        $("#autocomplete").ejmAutocomplete({ sortOrder: "Descending", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### templateId `String`
{:#members:templateid}

Specifies ID of the element that contains template contents.

#### Default Value: 

* “”

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-templateid="template" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering -->
    <input id="autocomplete" />
    <script>
        //To set the templateId API value
        $("#autocomplete").ejmAutocomplete({ templateId: "template", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### value `String`
{:#members:value}

Specifies the textbox value on initialization

#### Default Value: 

* ””

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-value="Text" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        //To set the value API value
        $("#autocomplete").ejmAutocomplete({ value: "Text", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}


### watermarkText `String`
{:#members:watermarktext}

Specifies the autocomplete watermark text that to be shown on autocomplete text box when it is empty

#### Default Value: 

* null

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-watermarktext="Search" data-ej-datasource="window.datasrc" data-ej-fields-text="name" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
    <input id="autocomplete" />	
    <script>
        //To set the watermarkText API value
        $("#autocomplete").ejmAutocomplete({ watermarkText: "Search", dataSource: "window.datasrc", fields: { text: "name" } });
    </script>


{% endhighlight %}



## Methods

### clearText()
{:#methods:cleartext}

Clears the selected items in AutoComplete

#### Example

{% highlight html %}

<input id="autocomplete" />
    <script>
        $(function () {
            // Clears text of autocomplete
            $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
            $("#autocomplete").ejmAutocomplete("clearText");
        });
    </script>


{% endhighlight %}

### disable()
{:#methods:disable}

To disable AutoComplete

#### Example

{% highlight html %}

<input id="autocomplete" />
    <script>
        $(function () {
            // Disable autocomplete
            $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
            $("#autocomplete").ejmAutocomplete("disable");
        });
    </script>


{% endhighlight %}


### enable()
{:#methods:enable}

To enable AutoComplete

#### Example

{% highlight html %}

<input id="autocomplete" />
    <script>
        $(function () {
            // Enable the autocomplete
            $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
            $("#autocomplete").ejmAutocomplete("enable");
        });
    </script>


{% endhighlight %}




### getSelectedItems()
{:#methods:getselecteditems}

To get the list of items selected in AutoComplete

#### Example

{% highlight html %}

<input id="autocomplete" />
    <script>
        $(function () {
            // GetSelectedItems of  autocomplete
            $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
            $("#autocomplete").ejmAutocomplete("getSelectedItems");
        });
    </script>


{% endhighlight %}


### getValue()
{:#methods:getvalue}

To get the value of AutoComplete

#### Example

{% highlight html %}

<input id="autocomplete" />
    <script>
        $(function () {
            // Getvalue of  autocomplete
            $("#autocomplete").ejmAutocomplete({ dataSource: "window.datasrc", fields: { text: "name" } });
            $("#autocomplete").ejmAutocomplete("getValue");
        });
    </script>


{% endhighlight %}


## Events



### change
{:#events:change}

Event triggers when the AutoComplete text box content changed.

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
Event parameters from autocomplete<table><br><tr><br><th>
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
model</td><td>
string</td><td>
Returns the autocomplete model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
Returns the current selected data</td></tr>
<tr>
<td>
index</td><td>
int</td><td>
Returns the selecteditem index</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns whether the current item is checked or not</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
  <input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" data-ej-change="onChange" />
    <script>
        // change event for autocomplete
        function onChange(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        $("#autocomplete").ejmAutocomplete({
            dataSource: "window.datasrc", fields: { text: "name" },
            change: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}


### focusIn
{:#events:focusin}

Event triggers when focused in to the Autocomplete text box

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
Event parameters from autocomplete<table><br><tr><br><th>
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
model</td><td>
string</td><td>
Returns the autocomplete model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
if the autocomplete textbox is interacted return true; otherwise return false</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" data-ej-focusin="onfocusIn" />
    <script>
        // focusIn event for autocomplete
        function onfocusIn(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        $("#autocomplete").ejmAutocomplete({
            dataSource: "window.datasrc", fields: { text: "name" },
            focusIn: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}


### focusOut
{:#events:focusout}

Event triggers when focused out from the Autocomplete text box

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
Event parameters from autocomplete<table><br><tr><br><th>
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
model</td><td>
string</td><td>
Returns the autocomplete model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
if the autocomplete textbox is interacted return true; otherwise return false</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" data-ej-focusout="onfocusOut" />
    <script>
        // focusOut event for autocomplete
        function onfocusOut(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        $("#autocomplete").ejmAutocomplete({
            dataSource: "window.datasrc", fields: { text: "name" },
            focusOut: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}


### keyPress
{:#events:keypress}

Event triggers when pressed a key

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
Event parameters from autocomplete<table><br><tr><br><th>
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
model</td><td>
string</td><td>
Returns the autocomplete model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
if the autocomplete textbox is interacted return true; otherwise return false</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" data-ej-keypress="onkeyPress" />
    <script>
        // keyPress event for autocomplete
        function onkeyPress(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        $("#autocomplete").ejmAutocomplete({
            dataSource: "window.datasrc", fields: { text: "name" },
            keyPress: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}


### select
{:#events:select}

Event triggers when we select an element from AutoComplete suggestion list.

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
Event parameters from autocomplete<table><br><tr><br><th>
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
model</td><td>
string</td><td>
Returns the autocomplete model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
element</td><td>
Object</td><td>
Returns the current element</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns whether the current item is checked or not</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Returns any item is selected or not</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" data-ej-select="onSelect" />
    <script>
        // select event for autocomplete
        function onSelect(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        $("#autocomplete").ejmAutocomplete({
            dataSource: "window.datasrc", fields: { text: "name" },
            select: function (args) {
                //handle the event                
            }
        });
    </script>


{% endhighlight %}





### touchEnd
{:#events:touchend}

Event triggers when the touch end happens in the AutoComplete suggestion list.

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
Event parameters from autocomplete<table><br><tr><br><th>
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
model</td><td>
string</td><td>
Returns the autocomplete model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
Returns the selected object</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Returns the current item text</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns whether the current item is checked or not</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Returns any item is selected or not</td></tr>
<tr>
<td>
isInteraction</td><td>
boolean</td><td>
if the autocomplete textbox is interacted return true; otherwise return false</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input id="autocomplete" data-role="ejmautocomplete" data-ej-datasource="window.datasrc" data-ej-fields-text="name" data-ej-touchend="onTouchEnd" />
    <script>
        // touchEnd event for autocomplete
        function onTouchEnd(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input id="autocomplete" />
    <script>
        $("#autocomplete").ejmAutocomplete({
            dataSource: "window.datasrc", fields: { text: "name" },
            touchEnd: function (args) {
                //handle the event
            }
        });
    </script>


{% endhighlight %}



























