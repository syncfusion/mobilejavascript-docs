---
layout: post
title: ejmGrid | API Reference | Mobile JS | Syncfusion
description: 
documentation: API
platform: Mobilejs
keywords: ejmGrid, API, Essential Studio JS Autocomplete (Mobile)
---

# ejmGrid

The Grid can be easily configured to the DOM element, div. You can create a Grid with a highly customizable look and feel.

$(element).ejmGrid<span class="signature">(options)</span>

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}options{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">settings for grid</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script> 
// Create Grid
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));   
$("#mobilegrid").ejmGrid({ dataSource:data,columns: [
		 { field: "OrderID", headerText: "Order ID" },
		 { field: "CustomerID", headerText: "Customer ID" },
		 { field: "Freight", headerText: "Freight" }
 ] });
 }); 
</script>{% endhighlight %}

#### Requires

* module:jQuery

* module:jsrender

* module:jquery.globalize

* module:ej.mobile.application

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch

* module:ej.mobile.scrollbar

* module:ej.mobile.scrollpanel

* module:ej.mobile.header

* module:ej.mobile.button

* module:ej.mobile.dialog

* module:ej.mobile.listbox

* module:ej.mobile.checkbox

## Members

### allowFiltering`boolean`
{:#members:allowfiltering}

Specifies whether to enable filtering for the columns. It allows to filter the desired records in Grid columns.


#### Default Value

* false

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ allowFiltering: false,dataSource:data,columns: [
			 { field: "OrderID", headerText: "Order ID" },
			 { field: "CustomerID", headerText: "Customer ID" },
			 { field: "Freight", headerText: "Freight" }
	 ] });
	 });    
</script>                                
{% endhighlight %}


### allowPaging`boolean`
{:#members:allowpaging}

Specifies whether to enable the pager feature in Grid.

#### Default Value

* false

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>  
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));                   
$("#mobilegrid").ejmGrid ({ allowPaging: true,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });                
</script>                                         {% endhighlight %}

### allowScrolling`boolean`
{:#members:allowscrolling}

Specifies whether to enable the scrolling feature in Grid.

#### Default Value

* false

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ allowScrolling: false,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>            {% endhighlight %}

### allowSelection`boolean`
{:#members:allowselection}

Specifies whether to enable the Grid row selection.

#### Default Value

* false

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ allowSelection: false,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>                                 {% endhighlight %}

### allowSorting`boolean`
{:#members:allowsorting}


Enables or disables the sorting behavior for Grid and you can sort the Grid columns in ascending or descending order.

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ allowSorting: false,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });
</script>                                {% endhighlight %}

### caption`string`
{:#members:caption}

Sets the caption for the Grid.

#### Default Value

* ""

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ caption: "caption", showCaption: true,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>                             {% endhighlight %}

### columns`array`
{:#members:columns}

It is used to define the columns that can be bound to Grid.

#### Default Value

* []

#### Example

{% highlight html %}<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejGrid({ dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });                   
</script> {% endhighlight %}

### cssClass`string`
{:#members:cssclass}

Specifies the CSS class to Grid to achieve custom theme.


#### Default Value

* ""

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script> 
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ cssClass: "Customclass",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>                                       {% endhighlight %}

### dataSource`data`
{:#members:datasource}

Specifies the data source for Grid.

#### Default Value

* null

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>                                 {% endhighlight %}

### enablePersistence`boolean`
{:#members:enablepersistence}

Specifies whether to enable the state maintenance in Grid.

#### Default Value

* false

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ enablePersistence: false,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>                     {% endhighlight %}

### filterSettings
{:#members:filtersettings}

To customize the filtering behavior of the Grid.

### filterSettings.filterBarMode`enum`
{:#members:filtersettings-filterbarmode}


Sets the filter bar mode option in the Grid. The accepted filterBarModes are "immediate" and "onenter". See <a href="global.html#FilterBarMode">FilterBarMode</a>

#### Default Value

* ej.mobile.Grid.FilterBarMode.OnEnter

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowFiltering:true,
                filterSettings: { filterBarMode: ej.mobile.Grid.FilterBarMode.OnEnter },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });           
</script>                                        {% endhighlight %}

### filterSettings.filteredColumns`object`
{:#members:filtersettings-filteredcolumns}

Gets filtered column details programmatically after filtering.

#### Default Value

* []

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowFiltering:true,
                filterSettings: { interval: 1500 },filteredColumns:[],dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });  
                 });            
</script>{% endhighlight %}

### filterSettings.interval`number`
{:#members:filtersettings-interval}

Specifies the filter interval in milliseconds when filterbar mode is set to Immediate.

#### Default Value

* 1500

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowFiltering:true,
                filterSettings: { interval: 1500 },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });  
                 });            
</script>                                        {% endhighlight %}

### pageSettings
{:#members:pagesettings}

This property is used to modify the default pager configuration.

### pageSettings.currentPage`number`
{:#members:pagesettings-currentpage}

This is used to define the page that has to be displayed currently.

#### Default Value

* 1

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowPaging:true,
                pageSettings: { currentPage: 1 },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });               
</script>                                 {% endhighlight %}

### pageSettings.display`enum`
{:#members:pagesettings-display}

Defines the pager position that can be fixed or normal. See <a href="global.html#PagerDisplay">PagerDisplay</a>

#### Default Value

* ej.mobile.Grid.PagerDisplay.Normal

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowPaging:true,
                pageSettings: { display: ej.mobile.Grid.PagerDisplay.Normal },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });              
</script>                                        {% endhighlight %}

### pageSettings.pageSize`number`
{:#members:pagesettings-pagesize}

Defines the number of records displayed per page.

#### Default Value

* 5


#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowPaging:true,
                pageSettings:{ pageSize: 5 },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });               
</script>                                 {% endhighlight %}


### pageSettings.totalRecordsCount`number`
{:#members:pagesettings-totalrecordscount}


It holds the total records count available in the Grid.

#### Default Value

* null

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
$("#mobilegrid").ejmGrid({
    dataSource:  window.gridData,
    allowPaging: true
});
});
var value = $("#mobilegrid").ejmGrid("option", "pageSettings.totalRecordsCount");
$("#print").text("TotalRecordsCount: " + value);             
</script>                                        {% endhighlight %}

### pageSettings.type`enum`
{:#members:pagesettings-type}

Defines the pager type, scrollable or normal. See <a href="global.html#PagerType">PagerType</a>

#### Default Value

* ej.mobile.Grid.PagerType.Scrollable

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowPaging:true,
                pageSettings:{ type: ej.mobile.Grid.PagerType.Scrollable },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });              
</script>                                         {% endhighlight %}

### renderMode`enum`
{:#members:rendermode}


Changes the rendering mode of the Grid. It can be auto, ios7, android, windows or flat. See <a href="global.html#RenderMode">RenderMode</a>


#### Default Value

* auto

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ renderMode: ej.mobile.RenderMode.Auto,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script> {% endhighlight %}

### scrollSettings
{:#members:scrollsettings}


Used to enable Grid column and row scrolling.

### scrollSettings.enableColumnScrolling`boolean`
{:#members:scrollsettings-enablecolumnscrolling}

Used to enable or disable column scrolling.

#### Default Value

* false

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowScrolling:true,
                scrollSettings:{ enableColumnScrolling: false },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });             
</script>                                  {% endhighlight %}

### scrollSettings.enableNativeScrolling`boolean`
{:#members:scrollsettings-enablenativescrolling}

Used to enable or disable native scrolling.

#### Default Value


* true

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script> 
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowScrolling:true,
                scrollSettings: { enableNativeScrolling: true },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });               
</script>                                {% endhighlight %}

### scrollSettings.enableRowScrolling`boolean`
{:#members:scrollsettings-enablerowscrolling}


Used to enable or disable row scrolling.

#### Default Value


* true

#### Example

{% highlight html %}  
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowScrolling:true,
                scrollSettings: { enableRowScrolling: true },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });  
                 });               
</script>                                          {% endhighlight %}

### scrollSettings.height`string`
{:#members:scrollsettings-height}

Specifies the height for the Grid content.


#### Default Value

* auto

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowScrolling:true,
                scrollSettings: { height: "auto" },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });  
                 });             
</script>                                 {% endhighlight %}




### selectedRowIndex`number`
{:#members:selectedrowindex}


To apply row selection based on your row index value.


#### Default Value

* -1

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
// Set grid selectedRowIndex on initialization. 
//To set selectedRowIndex API value 
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ selectedRowIndex: 1,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>                                       {% endhighlight %}

### sortSettings
{:#members:sortsettings}

This property is used to modify sorting default configuration.


### sortSettings.allowMultiSorting`boolean`
{:#members:sortsettings-allowmultisorting}

Enable or disable the multi sorting behavior of Grid.

#### Default Value

* false

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowSorting: true,
                sortSettings: { allowMultiSorting: false },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });   
                 });              
</script>                                          {% endhighlight %}

### sortSettings.sortedColumns`object`
{:#members:sortsettings-sortedcolumns}

To define the column that can be sorted and also to define the sort direction.

#### Default Value

* []

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ 
                allowSorting: true,
                sortSettings: { sortedColumns:[] },dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });  
                 });             
</script>                                          {% endhighlight %}

### theme`enum`
{:#members:theme}

Specifies the theme of the Grid. See <a href="global.html#Theme">Theme</a>

#### Default Value

* auto

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ theme: ej.mobile.Theme.Auto,dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });    
</script>                               {% endhighlight %}

### transition`string`

Specifies the transition type when navigation happens while interacting with Grid.

#### Default Value

* For Android, "pop". For Windows, "turn". For IOS, "slide".

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
// Set grid transition on initialization. 
//To set transition API value 
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid ({ transition: "slide",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });
</script>                              {% endhighlight %}

## Methods

### getColumnByField`()`
{:#methods:getcolumnbyfield}

To get column by field.

#### Example


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// Create grid object.
var gridObj = $("#mobilegrid").data("ejGrid");
gridObj.getColumnByField("OrderID"); // Get the column details based on the given field name
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// Get the column details based on the given field name
$("#mobilegrid").ejGrid("getColumnByField", "OrderID");        
</script>{% endhighlight %}


### getColumnByHeaderText`()`
{:#methods:getcolumnbyheadertext}


To get column by header text.

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>  
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.getColumnByHeaderText("Order ID"); // Get column by header text
</script>{% endhighlight %}


{% highlight html %} 
<div  id="mobilegrid" ></div>  
<script>
// Get column by header text
$("#mobilegrid").ejmGrid("getColumnByHeaderText", "Order ID");  
</script>{% endhighlight %}

### getColumnByIndex`()`
{:#methods:getcolumnbyindex}

To get column by index.


#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>        
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.getColumnByIndex(1); // Get column by index
</script>{% endhighlight %}


{% highlight html %} 
<div  id="mobilegrid" ></div>  
<script>
// Get column by index
$("#mobilegrid").ejmGrid("getColumnByIndex",1); 
</script>{% endhighlight %}


### getColumnFieldNames`()`
{:#methods:getcolumnfieldnames}


To get column field names.

#### Example


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.getColumnFieldNames(); // Get column field names
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// Get column field names
$("#mobilegrid").ejmGrid("getColumnFieldNames");        
</script>{% endhighlight %}

### getColumnIndexByField`()`
{:#methods:getcolumnindexbyfield}

To get column index by field.

#### Example


{% highlight html %} 
<div id="mobilegrid"></div>
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.getColumnIndexByField("OrderID"); // Get column index by field
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div>
<script>
// Get column index by field
$("#mobilegrid").ejmGrid("getColumnIndexByField","OrderID");    
</script>{% endhighlight %}


### getColumnMemberByIndex`()`
{:#methods:getcolumnmemberbyindex}

To get column member by index.

#### Example


{% highlight html %} 
<div id="mobilegrid"></div>
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.getColumnMemberByIndex(1); // Get column member by index
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div>
<script>
// Get column member by index
$("#mobilegrid").ejmGrid("getColumnMemberByIndex",1);   
</script>{% endhighlight %}


### hideColumns`()`
{:#methods:hidecolumns}

To hide the specified column.


#### Example


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.hideColumns("Order ID"); // Hides column based on the given header text of the column
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// Hides column based on the given header text of the column
$("#mobilegrid").ejmGrid("hideColumns","Order ID"); 
</script>{% endhighlight %}

### refreshContent`()`
{:#methods:refreshcontent}


It is used to refresh the Grid contents.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}[requestType].{% endhighlight %}</td>
<td class="type"><span class="param-type">enum</span></td>
<td class="description last">The request type can be refresh, paging, sorting, filtering. If no parameter is passed, the request type is refresh</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %} 
<div id="mobilegrid"></div>
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.refreshContent(); 
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div>
<script>
$("#mobilegrid").ejmGrid("refreshContent");     
</script>{% endhighlight %}


### scrollRefresh`()`
{:#methods:scrollrefresh}


To refresh Grid scroll panel.


#### Example


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.scrollRefresh(); // To Refresh grid scrollpanel
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div> 
<script>
// To Refresh grid scrollpanel
$("#mobilegrid").ejmGrid("scrollRefresh"); 
</script>{% endhighlight %}

### showColumns`()`
{:#methods:showcolumns}

To show the specified column.

#### Example

{% highlight html %} 
<div id="mobilegrid"></div>
<script>
// Create Grid
var grid = $("#mobilegrid").data("ejmGrid");
grid.showColumns("Order ID"); // Shows column based on the given header text of the column
</script>{% endhighlight %}


{% highlight html %} 
<div id="mobilegrid"></div>
<script>
// Shows column based on the given header text of the column
$("#mobilegrid").ejmGrid("showColumns","Order ID");     
</script>{% endhighlight %}

## Events

### actionBegin
{:#events:actionbegin}

Triggered for every Grid action before it starts.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}requestType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
//actionBegin event for grid
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ actionBegin:"actionBegin",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });            
function actionBegin(args) { //handle the event }                       
</script>                 {% endhighlight %}

### actionComplete
{:#events:actioncomplete}

Event triggers when loading action of Grid data succeeds.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}requestType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
//actionComplete event for grid
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ actionComplete:"actionComplete",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });
function actionComplete(args) { //handle the event }            
</script>                 {% endhighlight %}

### actionFailure
{:#events:actionfailure}

Event triggers when loading action of Grid data fails.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}requestType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ actionFailure:"actionFailure",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });
function actionFailure(args) { //handle the event }            
</script>                 {% endhighlight %}

### actionSuccess
{:#events:actionsuccess}

Triggered for every Grid action success.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}requestType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
//actionSuccess event for grid
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ actionSuccess:"actionSuccess",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });
function actionSuccess(args) { //handle the event }          
</script>                 {% endhighlight %}

### load
{:#events:load}

Triggered for every Grid load.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}requestType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ load:"load",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });
function load(args) { //handle the event }            
</script>                 {% endhighlight %}

### modelChange
{:#events:modelchange}

Triggered every time when a model value changes.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current Grid row.</td>
</tr>
<tr>
<td class="name">{% highlight html %}options{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the changed model values.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
//modelChange event for grid
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ modelChange:"modelChange",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 }); 
function modelChange(args) { //handle the event }            
</script>                 {% endhighlight %}

### queryCellInfo
{:#events:querycellinfo}

Triggered every time a request is made to access particular cell information, element and data.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current cell.</td>
</tr>
<tr>
<td class="name">{% highlight html %}data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current data.</td>
</tr>
<tr>
<td class="name">{% highlight html %}text{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current cell HTML content.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
//queryCellInfo event for grid
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ queryCellInfo:"queryCellInfo",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] }); 
                 });
function queryCellInfo(args) { //handle the event }   
</script>                         {% endhighlight %}

### rowDataBound
{:#events:rowdatabound}


Triggered every time a request is made to access row information, element and data.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current Grid row.td>
</tr>
<tr>
<td class="name">{% highlight html %}data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current data.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
//rowDataBound event for grid
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ rowDataBound:"rowDataBound",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 }); 
function rowDataBound(args) { //handle the event }              
</script>                         {% endhighlight %}

### rowSelected
{:#events:rowselected}

Triggered after the row is selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}rowIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the current row index.</td>
</tr>
<tr>
<td class="name">{% highlight html %}row{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current row.</td>
</tr>
<tr>
<td class="name">{% highlight html %}cell{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current data cell.</td>
</tr>
<tr>
<td class="name">{% highlight html %}data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current data record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));
$("#mobilegrid").ejmGrid({ rowSelected:"rowSelected",dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ] });
                 });                     
function rowSelected(args) { //handle the event }
</script>                 {% endhighlight %}

### rowSelecting
{:#events:rowselecting}

Triggered before the row is to be selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}argument{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Grid
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">{% highlight html %}cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the Grid model.</td>
</tr>
<tr>
<td class="name">{% highlight html %}type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">{% highlight html %}element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Returns the current element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}rowIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the current row index.</td>
</tr>
<tr>
<td class="name">{% highlight html %}row{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current row.</td>
</tr>
<tr>
<td class="name">{% highlight html %}cell{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current data cell.</td>
</tr>
<tr>
<td class="name">{% highlight html %}data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current data record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %} 
<div  id="mobilegrid" ></div>
<script>       
$(document).ready(function(){
var data = ej.DataManager(window.gridData).executeLocal(ej.Query().take(50));                   
$("#mobilegrid").ejmGrid ({ dataSource:data,columns: [
                         { field: "OrderID", headerText: "Order ID" },
                         { field: "CustomerID", headerText: "Customer ID" },
                         { field: "Freight", headerText: "Freight" }
                 ],rowSelecting:"rowSelecting" });
                 });    
function rowSelecting(args) { //handle the event }      
</script>                         {% endhighlight %}