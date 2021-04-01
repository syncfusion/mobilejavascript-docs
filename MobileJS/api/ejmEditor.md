---
layout: post
title: ejmEditor | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmEditor
platform: Mobilejs
control: ejmEditor
documentation: API
keywords: ejmEditor, API, Essential Studio JS Editor (Mobile) 
---


# ejmEditor

The Essential JavaScript Mobile Editor controls are used to display or get the value.


#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch



#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" />


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering -->
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox();
    </script>



{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" />


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering -->
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword();
    </script>



{% endhighlight %}

MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" />


{% endhighlight %}



{% highlight html %}

     <!-- Obtrusive way of rendering -->
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <textarea id="textarea" data-role="ejmtextarea"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea();
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric();
    </script>


{% endhighlight %}


## Members


### autoFocus `Boolean`
{:#members:autofocus}

Specifies the control  automatically get focus on initialization.

#### Default Value:

* false

#### Example

TextBox

{% highlight html %}

   <!-- Unobtrusive way of rendering -->
 <input id="textbox" data-role="ejmtextbox" data-ej-autofocus="true" />


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ autoFocus: true });
    </script>


{% endhighlight %}

Password

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
  <input id="password" data-role="ejmpassword" data-ej-autofocus="true" />


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering --> 
      <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ autoFocus: true });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
  <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-autofocus="true" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", autoFocus: true });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

   <!-- Unobtrusive way of rendering -->
 <textarea id="textarea" data-role="ejmtextarea" data-ej-autofocus="true"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ autoFocus: true });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-autofocus="true" />


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ autoFocus: true });
    </script>


{% endhighlight %}



### borderStyle `Enum`
{:#members:borderstyle}

Specifies the style of the border. See [BorderStyle](http://help.syncfusion.com/mobilejs/api/global#members:borderstyle)

#### Default Value:

* ”box”

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-borderstyle="line" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ borderStyle: "line" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
   <input id="password" data-role="ejmpassword" data-ej-borderstyle="line" />


{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ borderStyle: "line" });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-borderstyle="line" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", borderStyle: "line" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-borderstyle="line"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ borderStyle: "line" });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-borderstyle="line" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ borderStyle: "line" });
    </script>


{% endhighlight %}



### cssClass `String`
{:#members:cssclass}

Sets the root class for Editor theme. This cssClass API helps to use custom skinning option for Editor Control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value:

* ””

#### Example

TextBox



{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-cssclass="customclass" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ cssClass: "customclass" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
   <input id="password" data-role="ejmpassword" data-ej-cssclass="customclass" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ cssClass: "customClass" });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-cssclass="customclass" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", cssClass: "customclass" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-cssclass="customclass"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ cssClass: "customclass" });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-cssclass="customclass" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ cssClass: "customclass" });
    </script>


{% endhighlight %}



### enabled `Boolean`
{:#members:enabled}

Specifies whether to enable or disable the control.

#### Default Value:

* true

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-enabled=false />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        $("#textbox").ejmTextBox({ enabled: false });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej-enabled=false />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        $("#password").ejmPassword({ enabled: false });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej-enabled=false data-ej-format="+1 (999) 999-9999" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        $("#maskedit").ejmMaskEdit({ enabled: false, mask: "+1 (999) 999-9999" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-enabled=false></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        $("#textarea").ejmTextArea({ enabled: false });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-enabled=false />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input type="number" id="editor" />
    <script>
        $("#editor").ejmNumeric({ enabled: false });
    </script>


{% endhighlight %}



### enablePersistence `Boolean`
{:#members:enablepersistence}

Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.

#### Default Value:

* false

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-enablepersistence=false />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />	
    <script>
        $("#textbox").ejmTextBox({ enablePersistence: false });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej- enablepersistence =false />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        $("#password").ejmPassword({ enablePersistence: false });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej- enablepersistence =false data-ej-format="+1 (999) 999-9999" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        $("#maskedit").ejmMaskEdit({ enablePersistence: false, mask: "+1 (999) 999-9999" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej- enablepersistence =false></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>	
        $("#textarea").ejmTextArea({ enablePersistence: false });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej- enablepersistence =false />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input type="number" id="editor" />
    <script>
        $("#editor").ejmNumeric({ enablePersistence: false });
    </script>


{% endhighlight %}



### format `String`
{:#members:format}

Specifies the 'format' for maskedit.

#### Default Value:

* ””

#### Example

MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000" });
    </script>


{% endhighlight %}



### height `String`
{:#members:height}

Specifies the text area height on initialization.

#### Default Value:

* ””

#### Example



textarea

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <textarea id="textarea" data-role="ejmtextarea" data-ej-height="200"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ height: "200" });
    </script>


{% endhighlight %}



### locale `String`
{:#members:locale}

Change the Control text format based on given culture.

#### Default Value:

* “en-US”

#### Example

TextBox

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="textbox" data-role="ejmtextbox" data-ej-locale="en-US" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ locale: "en-US" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="password" data-role="ejmpassword" data-ej-locale="en-US" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ locale: "en-US" });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-locale="en-US" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", locale: "en-US" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-locale="en-US"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ locale: "en-US" });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-locale="en-US" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ locale: "en-US" });
    </script>


{% endhighlight %}



### maxLength `String`
{:#members:maxlength}

Specifies the maximum length on initialization.

#### Default Value:

* ””

#### Example

TextBox



{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-maxlength ="5" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ maxLength: "5" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej-maxlength ="5 " />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ maxLength: "5" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-maxlength ="5"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ maxLength: "5" });
    </script>


{% endhighlight %}



### maxValue `Int`
{:#members:maxvalue}

Specifies the maximum value of the numeric textbox.

#### Default Value:

* -(Number.MAX_VALUE)

#### Example

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-maxvalue="5" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ maxValue: 5 });
    </script>


{% endhighlight %}



### minValue `Int`
{:#members:minvalue}

Specifies the minimum value of the numeric textbox.

#### Default Value:

*  Number.MAX_VALUE

#### Example

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-minvalue="5" />


{% endhighlight %}





{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ minValue: 5 });
    </script>


{% endhighlight %}



### readOnly `Boolean`
{:#members:readonly}

Specifies whether to be 'readonly' on initialization.

#### Default Value:

* false

#### Example

TextBox

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-readonly=true />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        $("#textbox").ejmTextBox({ readOnly: true });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej-readonly=true />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        $("#password").ejmPassword({ readOnly: true });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej-readonly=true data-ej-format="+1 (999) 999-9999" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        $("#maskedit").ejmMaskEdit({ readOnly: true, mask: "+1 (999) 999-9999" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-readonly=true></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        $("#textarea").ejmTextArea({ readOnly: true });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-readonly=true />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input type="number" id="editor" />
    <script>
        $("#editor").ejmNumeric({ readOnly: true });
    </script>


{% endhighlight %}



N> In Numeric textbox Specifies whether the control is read only to disable typing the value manually rather than updating by spin button.

### renderMode `Enum`
{:#members:rendermode}

Specifies the rendering mode of the control. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#members:rendermode)

#### Default Value:

* auto

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-rendermode="android" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ renderMode: "android" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej-rendermode="android" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ renderMode: "android" });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-rendermode="android" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", renderMode: "android" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <textarea id="textarea" data-role="ejmtextarea" data-ej-rendermode="android"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ renderMode: "android" });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-rendermode="android" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ renderMode: "android" });
    </script>


{% endhighlight %}






### step `Int`
{:#members:step}

Specifies the step value of numeric textbox for increments / decrements.

#### Default Value:

* 1

#### Example

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-step="5" />


{% endhighlight %}





{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ step: 5 });
    </script>


{% endhighlight %}



### type `Enum`
{:#members:type}

Specifies the textbox type.see [Type](http://help.syncfusion.com/mobilejs/api/global#members:textboxtype)

#### Default Value:

* ”text”

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-type="tel" />


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ type: "tel" });
    </script>


{% endhighlight %}




### value `String`
{:#members:value}

Specifies the 'value' on initialization.

#### Default Value:

* ””

#### Example

TextBox

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="textbox" data-role="ejmtextbox" data-ej-value="Enter here" />


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ value: "Enter here" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="password" data-role="ejmpassword" data-ej-value="Enter here" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ value: "Enter here" });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-value="12/12/2012" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", value: "12/12/2012" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <textarea id="textarea" data-role="ejmtextarea" data-ej-value ="Enter here"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ value: "Enter here" });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-value="10" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ value: "10" });
    </script>


{% endhighlight %}



### watermarkText `String`
{:#members:watermarktext}

The text to be displayed when the value of the  textbox is empty.

#### Default Value:

* ””

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-watermarktext="Enter here" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ watermarkText: "Enter here" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="password" data-role="ejmpassword" data-ej-watermarktext="Enter here" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ watermarkText: "Enter here" });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-watermarktext="Enter here" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", watermarkText: "Enter here" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <textarea id="textarea" data-role="ejmtextarea" data-ej-watermarktext ="Enter here"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ watermarkText: "Enter here" });
    </script>


{% endhighlight %}



### width `String`
{:#members:width}

Specifies the width on initialization.

#### Default Value:

* ””

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
<input id="textbox" data-role="ejmtextbox" data-ej-width="200" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />
    <script>
        //Create the textbox
        $("#textbox").ejmTextBox({ width: "200" });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej-width="200" />


{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />
    <script>
        //Create the password
        $("#password").ejmPassword({ width: "200" });
    </script>
	
{% endhighlight %}	

MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-width="200" />

{% endhighlight %}

{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />
    <script>
        //Create the maskedit
        $("#maskedit").ejmMaskEdit({ format: "00/00/0000", width: "200" });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <textarea id="textarea" data-role="ejmtextarea" data-ej-width="200"></textarea>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <textarea id="textarea"></textarea>
    <script>
        //Create the textarea
        $("#textarea").ejmTextArea({ width: "200" });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

  <!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-width="200" />


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="editor" type="number" />
    <script>
        $("#editor").ejmNumeric({ width: "200" });
    </script>


{% endhighlight %}



## Events

### keyDown
{:#events:keydown}


Event triggers when the KeyDown happens on the control.

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
Event parameters.<table><br><tr><br><th>
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
Returns the value of the control</td></tr>
</table>


</td></tr>
</table>

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-keydown="keyDown" />

    <script>
        function keyDown(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering --> 
 <input id="textbox" />

    <script>
        $("#textbox").ejmTextBox({
            keyDown: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Password

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="password" data-role="ejmpassword" data-ej-keydown="keyDown" />

    <script>
        function keyDown(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

   <!-- Obtrusive way of rendering -->  
<input id="password" />

    <script>
        $("#password").ejmPassword({
            keyDown: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-keydown="keyDown" />

    <script>
        function keyDown(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

    <!-- Obtrusive way of rendering --> 
<input id="maskedit" />

    <script>
        $("#maskedit").ejmMaskEdit({
            format: "00/00/0000",
            keyDown: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-keydown="keyDown"></textarea>

    <script>
        function keyDown(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering --> 
  <textarea id="textarea"></textarea>

    <script>
        $("#textarea").ejmTextArea({
            keyDown: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input type="number" id="editor" data-role="ejmnumeric" data-ej-keydown="keyDown" />


    <script>
        function keyDown(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

  <!-- Obtrusive way of rendering --> 
  <input id="editor" type="number" />

    <script>
        $("#editor").ejmTextBox({
            keyDown: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### keyUp
{:#events:keyup}

Event triggers when the KeyUp happens on the control.

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
Event parameters.<table><br><tr><br><th>
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
Returns the value of the control</td></tr>
</table>


</td></tr>
</table>

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-keyup="keyUp" />

    <script>
        function keyUp(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="textbox" />

    <script>
        $("#textbox").ejmTextBox({
            keyUp: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Password

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="password" data-role="ejmpassword" data-ej-keyup="keyUp" />

    <script>
        function keyUp(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="password" />

    <script>
        $("#password").ejmPassword({
            keyUp: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-keyup="keyUp" />

    <script>
        function keyUp(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="maskedit" />

    <script>
        $("#maskedit").ejmMaskEdit({
            format: "00/00/0000",
            keyUp: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-keyup="keyUp"></textarea>

    <script>
        function keyUp(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <textarea id="textarea"></textarea>

    <script>
        $("#textarea").ejmTextArea({
            keyUp: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-keyup="keyUp" />


    <script>
        function keyUp(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="editor" type="number" />

    <script>
        $("#editor").ejmTextBox({
            keyUp: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### touchEnd
{:#events:touchend}

Event triggers when the TouchEnd happens on the control.

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
Event parameters.<table><br><tr><br><th>
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
Returns the value of the control</td></tr>
</table>


</td></tr>
</table>

#### Example

TextBox

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="textbox" data-role="ejmtextbox" data-ej-touchend="touchEnd" />

    <script>
        function touchEnd(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="textbox" />

    <script>
        $("#textbox").ejmTextBox({
            touchEnd: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej-touchend="touchEnd" />

    <script>
        function touchEnd(args) {
            //handle the event
        }
    </script>


{% endhighlight %}

{% highlight html %}

 <!-- Obtrusive way of rendering -->; 
   <input id="password" />
    <script>
        $("#password").ejmPassword({

            touchEnd: function (args) { //handle the event

            }
        });
    </script>

	{% endhighlight %}
	
MaskEdit

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-touchend="touchEnd" />

    <script>
        function touchEnd(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="maskedit" />

    <script>
        $("#maskedit").ejmMaskEdit({
            format: "00/00/0000",
            touchEnd: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-touchend="touchEnd"></textarea>

    <script>
        function touchEnd(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <textarea id="textarea"></textarea>

    <script>
        $("#textarea").ejmTextArea({
            touchEnd: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-touchend="touchEnd" />


    <script>
        function touchEnd(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="editor" type="number" />

    <script>
        $("#editor").ejmTextBox({
            touchEnd: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



### touchStart
{:#events:touchstart}

Event triggers when the TouchStart happens on the control.

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
Event parameters.<table><br><tr><br><th>
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
Returns the value of the control</td></tr>
</table>


</td></tr>
</table>

#### Example

TextBox

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="textbox" data-role="ejmtextbox" data-ej-touchstart="touchStart" />

    <script>
        function touchStart(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="textbox" />

    <script>
        $("#textbox").ejmTextBox({
            touchStart: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Password

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input id="password" data-role="ejmpassword" data-ej-touchstart="touchStart" />

    <script>
        function touchStart(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

<!-- Obtrusive way of rendering --> 
    <input id="password" />

    <script>
        $("#password").ejmPassword({
            touchStart: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

MaskEdit

{% highlight html %}

 <!-- Unobtrusive way of rendering -->
   <input id="maskedit" data-role="ejmmaskedit" data-ej-format="00/00/0000" data-ej-touchstart="touchStart" />

    <script>
        function touchStart(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="maskedit" />

    <script>
        $("#maskedit").ejmMaskEdit({
            format: "00/00/0000",
            touchStart: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

TextArea

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <textarea id="textarea" data-role="ejmtextarea" data-ej-touchstart="touchStart"></textarea>

    <script>
        function touchStart(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <textarea id="textarea"></textarea>

    <script>
        $("#textarea").ejmTextArea({
            touchStart: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}

Numeric

{% highlight html %}

<!-- Unobtrusive way of rendering -->
    <input type="number" id="editor" data-role="ejmnumeric" data-ej-touchstart="touchStart" />


    <script>
        function touchStart(args) {
            //handle the event
        }
    </script>


{% endhighlight %}



{% highlight html %}

 <!-- Obtrusive way of rendering --> 
   <input id="editor" type="number" />

    <script>
        $("#editor").ejmTextBox({
            touchStart: function (args) { //handle the event
            }
        });
    </script>


{% endhighlight %}



