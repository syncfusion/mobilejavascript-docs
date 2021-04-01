---
layout: post
title: ejmCheckBox | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmCheckBox
platform: Mobilejs
control: ejmCheckBox
documentation: API
keywords: ejmCheckBox, API, Essential Studio JS CheckBox (Mobile)
---

# ejmCheckBox

The Essential JavaScript Mobile widget for CheckBox element allows you to check an option or multiple options to perform an action, within your webpage and allows you to specify an option from the list.
Custom Design for Html CheckBox control.

Custom Design for HTML CheckBox control.

$(element).ejmCheckBox()

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" />
<script>
$("#chkbox").ejmCheckBox();
</script>


{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch


### checked `Boolean`
{:#members:checked}

Specifies whether to check the control.

#### Default Value: 

* false

#### Example


{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-checked=true />


{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" />
<script>
$("#chkbox").ejmCheckBox({ checked: true });
</script>


{% endhighlight %}

### cssClass `String`
{:#members:cssclass}

Sets the root class for CheckBox theme. This cssClass API helps to use custom skinning option for CheckBox control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value: 

* ””

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-cssclass="customclass" />


{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" />
<script>
// To set cssClass API value
$("#chkbox").ejmCheckBox({ cssClass: "customclass" });
</script>


{% endhighlight %}

### enabled `Boolean`
{:#members:enabled}

Specifies whether to enable or disable the control.

#### Default Value: 

* true

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-enabled=false />


{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" />
<script>
// To set enabled API value
$("#chkbox").ejmCheckBox({ enabled: false });
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
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-enablepersistence=true />


{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" />
<script>
$("#chkbox").ejmCheckBox({ enablePersistence: true });
</script>

{% endhighlight %}

### enableRippleEffect `Boolean`
{:#members:enablerippleeffect}

Specifies the ripple effect for the CheckBox control. By default in android mode its value is true and other rendermode we need to set as true.

#### Default Value: 

* ej.isAndroid()?true:false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-enablerippleeffect=true />


{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" />
<script>
$("#chkbox").ejmCheckBox({ enableRippleEffect: true });
</script>

{% endhighlight %}

### renderMode `enum`
{:#members:rendermode}

Specifies the rendering mode of the control.See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value: 

* auto

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-rendermode="auto" />


{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" />
<script>
// To set renderMode API value
$("#chkbox").ejmCheckBox({ renderMode: ej.mobile.RenderMode.Auto });
</script>

{% endhighlight %}


## Methods

### disable()
{:#methods:disable}
To disable the CheckBox.

#### Example

{% highlight html %}

<input type="checkbox" id="chkbox" />
<script>
// get the CheckBox current state
$("#chkbox").ejmCheckBox();
$("#chkbox").ejmCheckBox("disable");
</script>

{% endhighlight %}


### enable()
{:#methods:enable}
To enable the CheckBox.

#### Example

{% highlight html %}

<input type="checkbox" id="chkbox" />
<script>
$("#chkbox").ejmCheckBox();
$("#chkbox").ejmCheckBox("enable");
</script>

{% endhighlight %}

### isChecked()
{:#methods:ischecked}
To check whether the CheckBox is checked or not.

#### Example

{% highlight html %}

<input type="checkbox" id="chkbox" />
<script>
// get the CheckBox current state
$("#chkbox").ejmCheckBox();
$("#chkbox").ejmCheckBox("isChecked");
</script>


{% endhighlight %}

## Events

### beforeChange
{:#events:beforechange}

Event triggers before the CheckBox state is changed.

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
Event parameters from CheckBox.<table><br><tr><br><th>
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
value</td><td>
string</td><td>
Returns the current element associated value.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the status of the control.</td></tr>
<tr>
<td>
controlType</td><td>
string</td><td>
Returns the name of the control type</td></tr>
<tr>
<td>
element</td><td>
Object</td><td>
Returns the current CheckBox element</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-beforechange="onBeforeChange" />
<script>
// before change event for CheckBox
function onBeforeChange(args) {
//handle the event            
}
</script>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" />
// before change event for CheckBox
<script>
$("#chkbox").ejmCheckBox({
beforeChange: function (args) {
//handle the event                
}
});
</script>

{% endhighlight %}


### change
{:#events:change}

Event triggers when the CheckBox state is changed.

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
Event parameters from CheckBox.<table><br><tr><br><th>
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
value</td><td>
string</td><td>
Returns the current element associated value.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the status of the control.</td></tr>
<tr>
<td>
controlType</td><td>
string</td><td>
Returns the name of the control type</td></tr>
<tr>
<td>
element</td><td>
Object</td><td>
return the current CheckBox element</td></tr>
</table>

</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-change="onChange" />
<script>
// change event for CheckBox
function onChange(args) {
//handle the event
}
</script>


{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" />
// change event for CheckBox
<script>
$("#chkbox").ejmCheckBox({
change: function (args) {
//handle the event
}
});
</script>

{% endhighlight %}

### touchEnd
{:#events:touchend}

Event triggers when touch end happens on the control.

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
Event parameters from CheckBox.<table><br><tr><br><th>
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
value</td><td>
boolean</td><td>
Returns the current element associated value.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the status of the control.</td></tr>
</table>

</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-touchend="touchEnd" />
<script>
// touchEnd event for CheckBox
function touchEnd(args) {
//handle the event
}
</script>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" />
// touchEnd event for CheckBox
<script>
$("#chkbox").ejmCheckBox({
touchEnd: function (args) {
//handle the event
}
});
</script>

{% endhighlight %}

### touchStart
{:#events:touchstart}

Event triggers when touch start happens on the control.

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
Event parameters from CheckBox.<table><br><tr><br><th>
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
value</td><td>
string</td><td>
Returns the current element associated value.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Returns the status of the control.</td></tr>
<tr>
<td>
controlType</td><td>
string</td><td>
Returns the name of the control type</td></tr>
<tr>
<td>
element</td><td>
Object</td><td>
Returns the current CheckBox element</td></tr>
</table>

</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" data-ej-touchstart="touchStart" />
<script>
// touchStart event for CheckBox
function touchStart(args) {
//handle the event
}
</script>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="checkbox" id="chkbox" data-role="ejmcheckbox" />
// touchStart event for CheckBox
<script>
$("#chkbox").ejmCheckBox({
touchStart: function (args) {
//handle the event
}
});
</script>

{% endhighlight %}

































