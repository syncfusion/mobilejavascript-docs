---
layout: post
title: ejmRadioButton | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmRadioButton
platform: Mobilejs
control: ejmRadioButton
documentation: API
keywords: ejmRadioButton, API, Essential Studio JS RadioButton (Mobile) 
---

# ejmRadioButton


The Essential JavaScript Mobile RadioButton control allows you to choose an option to perform an action. This control allows you to select true/false. 

Custom Design for HTML RadioButton control.

$(element).ejmRadioButton()

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" />

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" />
<script>
$("#radbtn").ejmRadioButton();
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

### checked `Boolean`
{:#members:checked}

Specifies whether to check the control.

#### Default Value:

* false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-checked=true />

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" />
<script>
$("#radbtn").ejmRadioButton({ checked: true });
</script>

{% endhighlight %}

### cssClass `String`
{:#members:cssclass}

Sets the root class for RadioButton theme. This cssClass API helps to use custom skinning option for RadioButton control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* ””

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-cssclass="customclass" />

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" />
<script>
// To set cssClass API value
$("#radbtn").ejmRadioButton({ cssClass: "customclass" });
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
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-enabled=false />

{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" />
<script>
// To set enabled API value
$("#radbtn").ejmRadioButton({ enabled: false });
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
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-enablepersistence=true />

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" />
<script>
$("#radbtn").ejmRadioButton({ enablePersistence: true });
</script>

{% endhighlight %}

### enableRippleEffect `Boolean`
{:#members:enablerippleeffect}

Specifies the ripple effect for the RadioButton control. By default in android mode its value is true and other rendermode we need to set as true.

#### Default Value:

* ej.isAndroid()?true:false

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-enablerippleeffect=true />

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" />
<script>
$("#radbtn").ejmRadioButton({ enableRippleEffect: true });
</script>

{% endhighlight %}

### renderMode `Enum`
{:#members:rendermode}

Specifies the rendering mode of the control. See[RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value:

* auto

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-rendermode="auto" />

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" />
<script>
// To set renderMode API value
$("#radbtn").ejmRadioButton({ renderMode: ej.mobile.RenderMode.Auto });
</script>

{% endhighlight %}

## Methods

### disable()
{:#methods:disable}

To disable the radiobutton.

#### Example

{% highlight html %}

<input type="radio" id="radbtn" />
<script>
// get the radiobutton current state
$("#radbtn").ejmRadioButton();
$("#radbtn").ejmRadioButton("disable");
</script>

{% endhighlight %}

### enable()
{:#methods:enable}

To enable the radiobutton.

#### Example

{% highlight html %}

<input type="radio" id="radbtn" />
<script>
$("#radbtn").ejmRadioButton();
$("#radbtn").ejmRadioButton("enable");
</script>

{% endhighlight %}

### isChecked()
{:#methods:ischecked}

To check whether the radio button is checked or not.

#### Example

{% highlight html %}

<input type="radio" id="radbtn" />
<script>
// get the radiobutton current state
$("#radbtn").ejmRadioButton();
$("#radbtn").ejmRadioButton("isChecked");
</script>

{% endhighlight %}

## Events

### beforeChange
{:#events:beforechange}

Event triggers before the RadioButton state is changed.

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
Event parameters from RadioButton.<table><br><tr><br><th><br><b>Name</b></th><th>
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
Returns the name of the controltype</td></tr>
<tr>
<td>
element</td><td>
Object</td><td>
Returns the current radiobutton element</td></tr>
</table>

</td></tr>
</table>

#### Example  

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-beforechange="onBeforeChange" />
<script>
// before change event for radiobutton
function onBeforeChange(args) {
//handle the event            
}
</script>

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" />
// before change event for radiobutton
<script>
$("#radbtn").ejmRadioButton({
beforeChange: function (args) {
//handle the event                
}
});
</script>

{% endhighlight %}

### change
{:#events:change}

Event triggers when the RadioButton state is changed.

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
Event parameters from RadioButton.<table><br><tr><br><th><br><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
returns true if the event should be cancelled; otherwise, false.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
returns the name of the event.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
returns the model value of the control.</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
returns the current element associated value.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
returns the status of the control.</td></tr>
<tr>
<td>
controlType</td><td>
string</td><td>
returns the name of the controltype</td></tr>
<tr>
<td>
element</td><td>
Object</td><td>
return the current radiobutton element</td></tr>
</table>

</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-change="onChange" />
<script>
// change event for radiobutton
function onChange(args) {
//handle the event
}
</script>

{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" />
// change event for radiobutton
<script>
$("#radbtn").ejmRadioButton({
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
Event parameters from RadioButton.<table><br><tr><br><th><br><b>Name</b></th><th>
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
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-touchend="touchend" />
<script>
// touchEnd event for radiobutton
function touchend(args) {
//handle the event
}
</script>

{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" />
// touchEnd event for radiobutton
<script>
$("#radbtn").ejmRadioButton({
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
Event parameters from Radiobutton.<table><br><tr><br><th><br><b>Name</b></th><th>
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
Returns the name of the controltype</td></tr>
<tr>
<td>
element</td><td>
Object</td><td>
Return the current radiobutton element</td></tr>
</table>

</td></tr>
</table>

#### Example

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" data-ej-touchstart="touchstart" />
<script>
// touchStart event for radiobutton
function touchstart(args) {
//handle the event
}
</script>

{% endhighlight %}


{% highlight html %}

<!-- Obtrusive way of rendering -->
<input type="radio" id="radbtn" data-role="ejmradiobutton" />
// touchStart event for radiobutton
<script>
$("#radbtn").ejmRadioButton({
touchStart: function (args) {
//handle the event
}
});
</script>


{% endhighlight %}
































