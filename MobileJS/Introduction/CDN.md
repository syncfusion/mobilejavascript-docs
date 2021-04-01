---
layout: post
title: CDN | Introduction | Mobilejs | Syncfusion
description: cdn
platform: Mobilejs
control: Introduction
documentation: ug
---

# CDN

The [CDN](http://en.wikipedia.org/wiki/Content_delivery_network) links are provided individually for all the Scripts and Stylesheets that provide easier access to Syncfusion JavaScript components.

N> All the provided CDN used either through http or https.



## CDN Script links



### External dependency libraries



The first three common script libraries listed in the following table are more essential and mandatory to render any of the Syncfusion widgets on the application module. The basic syntax is as follows,

{% highlight text %}

http://cdn.syncfusion.com/js/assets/external/[file name]  
    Example: [http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js](http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js)


{% endhighlight %}

_Property Table_

<table>
<tr>
<td>
<b>Name</b></td><td>
<b>Details</b></td><td>
<b>CDN link</b></td></tr>
<tr>
<td>
jQuery 2.1.4</td><td>
Common jQuery script to render any of the Syncfusion widgets.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/jquery-2.1.4.min.js>http://cdn.syncfusion.com/js/assets/external/jquery-2.1.4.min.js</a> </td></tr>
<tr>
<td>
jsrender</td><td>
Supports template rendering.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/jsrender.min.js>http://cdn.syncfusion.com/js/assets/external/jsrender.min.js</a></td></tr>
<tr>
<td>
jQuery.Globalize</td><td>
Supports Globalization.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js>http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js</a></td></tr>
<tr>
<td>
Angular JS</td><td>
Minified angular file to support custom directives.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/angular.min.js>http://cdn.syncfusion.com/js/assets/external/angular.min.js</a></td></tr>
<tr>
<td>
excanvas</td><td>
To support canvas element rendering in IE8 browser.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/excanvas.min.js>http://cdn.syncfusion.com/js/assets/external/excanvas.min.js</a></td></tr>
<tr>
<td>
Knockout JS</td><td>
Minified knockout file to support the observable binding.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/knockout.min.js>http://cdn.syncfusion.com/js/assets/external/knockout.min.js</a></td></tr>
<tr>
<td>
requireJS</td><td>
Supports loading of required dependencies.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/require.min.js>http://cdn.syncfusion.com/js/assets/external/require.min.js</a></td></tr>
<tr>
<td>
jquery.validate</td><td>
Supports client-side validation.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/jquery.validate.min.js>http://cdn.syncfusion.com/js/assets/external/jquery.validate.min.js</a></td></tr>
<tr>
<td>
Jquery.validate.unobtrusive</td><td>
To enable unobtrusive validation options in data-* attributes.</td><td>
<a href=http://cdn.syncfusion.com/js/assets/external/jquery.validate.unobtrusive.min.js>http://cdn.syncfusion.com/js/assets/external/jquery.validate.unobtrusive.min.js</a></td></tr>
</table>



### Syncfusion Dependency Libraries - Based on latest build version

The CDN script files are maintained for each version of the Essential Studio individually. Refer to the following syntax.

{% highlight text %}

http://cdn.syncfusion.com/[version]/js/mobile/[file name] 
    For example, to access the ej.mobile.all.min.js file in 14.1.0.46 version– 
    [https://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.js]([https://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.js](https://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.js))


{% endhighlight %}


_Property Table_

<table>
<tr>
<td>
<b>Name</b></td><td>
<b>Details</b></td><td>
<b>CDN link</b></td></tr>
<tr>
<td>
ej.mobile.all.min</td><td>
Combined script file that includes the script of all the Syncfusion UI mobile widgets.</td><td>
<a href=http://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.js>http://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.js</a></td></tr>
<tr>
<td>
ej.unobtrusive.min</td><td>
Supports Syncfusion widgets to render in HTML5 format.</td><td>
<a href=http://cdn.syncfusion.com/14.1.0.46/js/web/ej.unobtrusive.min.js>http://cdn.syncfusion.com/14.1.0.46/js/web/ej.unobtrusive.min.js</a></td></tr>
<tr>
<td>
ej.widget.angular.min</td><td>
Provides complete support for Angular JS.</td><td>
<a href=http://cdn.syncfusion.com/14.1.0.46/js/ej.widget.angular.min.js>http://cdn.syncfusion.com/14.1.0.46/js/ej.widget.angular.min.js</a></td></tr>
<tr>
<td>
ej.widget.ko.min</td><td>
Provides complete support for Knockout JS.</td><td>
<a href=http://cdn.syncfusion.com/14.1.0.46/js/ej.widget.ko.min.js>http://cdn.syncfusion.com/14.1.0.46/js/ej.widget.ko.min.js</a></td></tr>
</table>
The Knockout and angular dependencies can be accessed through the following syntax,

{% highlight text %}

http://cdn.syncfusion.com/[version]/js/[file name]
    For example, to access the ej.widget.angular.min.js file in 14.1.0.46 version– 
    [https://cdn.syncfusion.com/14.1.0.46/js/ej.widget.angular.min.js]([https://cdn.syncfusion.com/14.1.0.46/js/ej.widget.angular.min.js](https://cdn.syncfusion.com/14.1.0.46/js/ej.widget.angular.min.js))


{% endhighlight %}


## CDN Stylesheet links

The CDN links for all the CSS files (both core & theme related) are depicted together in the following table. Refer to the following syntax:

{% highlight text %}

http://cdn.syncfusion.com/[version]/js/mobile/[file name]


{% endhighlight %}

_Property Table_

<table>
<tr>
<td>
<b>Name</b></td><td>
<b>Details</b></td><td colspan = "2">
<b>CDN link</b></td></tr>
<tr>
<td>
ej.mobile.all.min.css</td><td colspan = "2">
Includes the CSS of all the themes combined in a single CSS file.</td><td>
<a href=http://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.css>http://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.css</a></td></tr>
</table>




## Referring local Scripts & CSS, when CDN fails

Sometimes, CDN links may go down due to network or connection problems. On such scenarios, you can refer to the local scripts and CSS files dynamically in the application by checking if the scripts and CSS files loaded through CDN returns undefined. If it returns undefined, the local scripts get referred, else the CDN links work fine as illustrated in the following code example.

{% highlight html %}

<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
    <title>My first HTML page</title> <!-- CDN LINK references-->
    <link href="http://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js"></script>
    <script src="http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js"></script>
    <script src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
    <script src="http://cdn.syncfusion.com/14.1.0.46/js/mobile/ej.mobile.all.min.js"></script>
    <script type="text/javascript">
        if (typeof jQuery == "undefined") {
            // If CDN fails, jQuery returns undefined
            // Referring local scripts - Specify the path where the following files are located in your machine
            document.write(decodeURIComponent('%3Cscript src="Scripts/jquery-1.10.2.min.js" %3E%3C/script%3E'));
            document.write(decodeURIComponent('%3Cscript src="Scripts/jquery.globalize.min.js" %3E%3C/script%3E'));
            document.write(decodeURIComponent('%3Cscript src="Scripts/jsrender.min.js" %3E%3C/script%3E'));
        }
        if (typeof ej == "undefined") {
            // If CDN fails, ej returns undefined.
            // So that, refer the Syncfusion stylesheets and scripts from the local path here
            // StyleSheet reference from the local system path
            document.write(decodeURIComponent('%3Clink rel="stylesheet" href="Content/ej/mobile/ej.mobile.all.min.css" %3C/%3E'));
            // Script reference from the local system path
            document.write(decodeURIComponent('%3Cscript src="Scripts/ej/ej.mobile.all.min.js" %3E%3C/script%3E'));
        }
    </script>
</head>
<body>
    <div data-role="appview">
        <!--Container for ejmDatePicker widget-->
        <input id="startDate" data-role="ejmdatepicker" />
    </div>
</body>
</html>


{% endhighlight %}



