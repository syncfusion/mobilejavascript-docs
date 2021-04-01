---
layout: post
title: ejmRadialMenu | API Reference | Mobile JS | Syncfusion
description:  Methods, members, events available in ejmRadialMenu
platform: Mobilejs
control: ejmRadialMenu
documentation: API
keywords: ejmRadialMenu, API, Essential Studio JS RadialMenu (Mobile)
---

# ejmRadialMenu

Essential JavaScript Mobile RadialMenu control is a context that represent the menu items in a circular order with a center button element in it.

Custom Design for HTML RadialMenu control.

$(element).ejmRadialMenu()

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="defaultradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        $("#defaultradialmenu").ejmRadialMenu();
    </script>



{% endhighlight %}



N> Provide proper image path to get images in items of RadialMenu.

#### Requires

* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.mobile.core

* module:ej.data

* module:ej.touch


## Members

### backImageClass `string`
{:#members:backimageclass} 

Renders the back button Image for center radial using class.

#### Default Value

* “e-m-backimage”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    
    <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-position="leftcenter" data-ej-imageclass="imageclass" data-ej-backimageclass="backimage">
        <ul>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/music.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/social.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/googleplus.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/facebook.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/direction.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/browser.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/chrome.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/opera.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/bing.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/message.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/google.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
        </ul>
    </div>
    <style type="text/css">
        .imageclass {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/home.png");
            background-position: center;
            background-repeat: no-repeat;
        }

        .backimage {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/windowsback.png");
            background-position: center;
            background-repeat: no-repeat;
            -moz-transform: scaleX(-1);
            -o-transform: scaleX(-1);
            -webkit-transform: scaleX(-1);
            transform: scaleX(-1);
            filter: FlipH;
            -ms-filter: "FlipH";
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->

<div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/music.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/social.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/googleplus.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/facebook.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/direction.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/browser.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/chrome.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/opera.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/bing.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/message.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/google.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
        </ul>
    </div>

    <script>
        $("#defaultradialmenu").ejmRadialMenu({ backImageClass: "backimage",imageClass="imageclass" }); 
    </script>

    <style type="text/css">
        .imageclass {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/home.png");
            background-position: center;
            background-repeat: no-repeat;
        }

        .backimage {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/windowsback.png");
            background-position: center;
            background-repeat: no-repeat;
            -moz-transform: scaleX(-1);
            -o-transform: scaleX(-1);
            -webkit-transform: scaleX(-1);
            transform: scaleX(-1);
            filter: FlipH;
            -ms-filter: "FlipH";
        }
    </style>

{% endhighlight %}



### cssClass `string`
{:#members:cssclass} 

Sets the root class for RadialMenu theme. This cssClass API helps to use custom skinning option for RadialMenu control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ””

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
       <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-cssclass="customclass">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

      <style>
        .customclass .e-m-radial {
            background-color: blue;
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="defaultradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

      <style>
        .customclass .e-m-radial {
            background-color: blue;
        }
    </style>
    <style>
        .customclass .e-m-radial {
            background-color: blue;
        }
    </style>

    <script>
        $("#defaultradialmenu").ejmRadialMenu({ cssClass: "customclass" });
    </script>



{% endhighlight %}



### enableAnimation `boolean`
{:#members:enableanimation} 

To enable Animation for RadialMenu.

#### Default Value

* true

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-enableanimation="false">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="defaultradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        $("#defaultradialmenu").ejmRadialMenu({ enableAnimation: "false" }); 
    </script>



{% endhighlight %}



### imageClass `string`
{:#members:imageclass} 

Renders the image for center radial using Class.

#### Default Value

* “e-m-radialimage”

#### Example


{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    
    <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-position="leftcenter" data-ej-imageclass="imageclass" data-ej-backimageclass="backimage">
        <ul>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/music.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/social.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/googleplus.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/facebook.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/direction.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/browser.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/chrome.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/opera.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/bing.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/message.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/google.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
        </ul>
    </div>
    <style type="text/css">
        .imageclass {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/home.png");
            background-position: center;
            background-repeat: no-repeat;
        }

        .backimage {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/windowsback.png");
            background-position: center;
            background-repeat: no-repeat;
            -moz-transform: scaleX(-1);
            -o-transform: scaleX(-1);
            -webkit-transform: scaleX(-1);
            transform: scaleX(-1);
            filter: FlipH;
            -ms-filter: "FlipH";
        }
    </style>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->

<div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/music.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/social.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/googleplus.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/facebook.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/direction.png">
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/browser.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/chrome.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/opera.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/bing.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
            <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/message.png">
                <ul>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/google.png">
                    </li>
                    <li data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/ios7/light/yahoo.png">
                    </li>
                </ul>
            </li>
        </ul>
    </div>

    <script>
        $("#defaultradialmenu").ejmRadialMenu({ backImageClass: "backimage",imageClass="imageclass" }); 
    </script>

    <style type="text/css">
        .imageclass {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/home.png");
            background-position: center;
            background-repeat: no-repeat;
        }

        .backimage {
            background: url("http://js.syncfusion.com/UG/Mobile/Content/radial/windowsback.png");
            background-position: center;
            background-repeat: no-repeat;
            -moz-transform: scaleX(-1);
            -o-transform: scaleX(-1);
            -webkit-transform: scaleX(-1);
            transform: scaleX(-1);
            filter: FlipH;
            -ms-filter: "FlipH";
        }
    </style>

{% endhighlight %}



### items `objectarray`
{:#members:items} 

Renders the RadialMenu using datasource which contains array of items.

#### Default Value

* []

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-items="[{ imagename: 'social.png', windows: { text: 'social' } }, { imagename: 'music.png' , windows: { text :'music' } }, { imagename: 'direction.png', windows: { text: 'direction' } }, { imagename: 'message.png', windows: { text: 'message' } }, { imagename: 'browser.png' , windows: { text :'browser' } }]">
    </div>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->

    <div id="defaultradialmenu"></div>
    <script>
        $("#defaultradialmenu").ejmRadialMenu({ items: [{ imagename: 'social.png', windows: { text: 'social' } }, { imagename: 'music.png', windows: { text: 'music' } }, { imagename: 'direction.png', windows: { text: 'direction' } }, { imagename: 'message.png', windows: { text: 'message' } }, { imagename: 'browser.png', windows: { text: 'browser' } }] });
    </script> 



{% endhighlight %}



### position `enum`
{:#members:position} 

Changes the Position of the control. See [RadialMenuPosition](http://help.syncfusion.com/mobilejs/api/global#radialmenuposition)

#### Default Value

* “rightcenter”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->

    <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-position="leftcenter">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="defaultradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>
    <script>
        $("#defaultradialmenu").ejmRadialMenu({ position: "leftcenter" }); 
    </script>



{% endhighlight %}



### radius `int`
{:#members:radius} 

Specifies the radius of the radialmenu control.

#### Default Value

* 150

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->

    <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-radius="100">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
       <div id="defaultradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>
    <script>
        $("#defaultradialmenu").ejmRadialMenu({ radius: 100 }); 
    </script>



{% endhighlight %}



### renderMode `enum`
{:#members:rendermode} 

Changes the rendering mode. See [RenderMode](http://help.syncfusion.com/mobilejs/api/global#rendermode)

#### Default Value

* “auto”

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
    <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-rendermode="android">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>


{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
    <div id="defaultradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        $("#defaultradialmenu").ejmRadialMenu({ renderMode: "android" }); 
    </script>



{% endhighlight %}



## Methods


### disableItemByIndex()
{:#methods:disableitembyindex} 

To disable an item of radialmenu by its index

#### Example

{% highlight html %}


    <div>
        <br />
        Click the button to disable the item in index 2
        <button data-role="ejmbutton" data-ej-touchend="disableItem">Disable Item</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function disableItem() {
            $("#defaultradialmenu").ejmRadialMenu("disableItemByIndex", 2)
        }
    </script>



{% endhighlight %}



### disableItemsByIndices()
{:#methods:disableitemsbyindices} 

To disable a set of radialmenu items by array of indices

#### Example

{% highlight html %}


    <div>
        <br />
        Click the button to disable the items in indices 2, 3 <button data-role="ejmbutton" data-ej-touchend="disableItems">Disable Items</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function disableItems() {
            $("#defaultradialmenu").ejmRadialMenu("disableItemsByIndices", [2,3])
        }
    </script>



{% endhighlight %}



### enableItemByIndex()
{:#methods:enableitembyindex} 

To enable a radialmenu item by its index

#### Example

{% highlight html %}


    <div>
        <br />
        Click the button to enable the item in index 2 <button data-role="ejmbutton" data-ej-touchend="enableItem">Enable Item</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function enableItem() {
            $("#defaultradialmenu").ejmRadialMenu("enableItemByIndex", 2)
        }
    </script>



{% endhighlight %}



### enableItemsByIndices()
{:#methods:enableitemsbyindices} 

To enable a set of radialmenu items by array of indices

#### Example

{% highlight html %}


    <div>
        <br />
        Click the button to enable the items in indices 2, 3 <button data-role="ejmbutton" data-ej-touchend="enableItems">Enable Items</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function enableItems() {
            $("#defaultradialmenu").ejmRadialMenu("enableItemsByIndices", [2,3])
        }
    </script>



{% endhighlight %}



### hide()

To hide the radialmenu with its target. You can’t access radialmenu after this method called.

Example

{% highlight html %}


    <div>
        <br />
        <button data-role="ejmbutton" data-ej-touchend="hide">Hide RadialMenu</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function hide() {
            $("#defaultradialmenu").ejmRadialMenu("hide");
        }
    </script>


{% endhighlight %}



### hideBadge()
{:#methods:hidebadge} 

To hide the radialmenu item’s badge by its index

#### Example

{% highlight html %}


    <div>
        <br />
        Click the button to hide badge value of item in index 2
        <button data-role="ejmbutton" data-ej-touchend="hideBadge">Hide Badge</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-imagename="social.png" data-ej-badge-value="10" data-ej-badge-enabled="true" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="social"></li>
            <li data-ej-imagename="music.png" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="music"></li>
            <li data-ej-imagename="direction.png" data-ej-badge-value="33" data-ej-badge-enabled="true" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="direction"></li>
            <li data-ej-imagename="message.png" data-ej-badge-value="5" data-ej-badge-enabled="true" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="message"></li>
            <li data-ej-imagename="browser.png" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="browser"></li>
        </ul>
    </div>

    <script>
        function hideBadge() {
            $("#defaultradialmenu").ejmRadialMenu("hideBadge", 2)
        }
    </script>



{% endhighlight %}



### hideMenu()
{:#methods:hidemenu} 

To hide the radialmenu when the target clicked

#### Example

{% highlight html %}


    <div>
        <br />
        <button data-role="ejmbutton" data-ej-touchend="hide">Hide RadialMenu</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function hide() {
            $("#defaultradialmenu").ejmRadialMenu("hideMenu");
        }
    </script>



{% endhighlight %}



### show()
{:#methods:show} 

To show the hidden RadialMenu control.

#### Example

{% highlight html %}



    <div>
        <br />
        <button data-role="ejmbutton" data-ej-touchend="show">Hide RadialMenu</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function show() {
            $("#defaultradialmenu").ejmRadialMenu("show");
        }
    </script>



{% endhighlight %}



### showBadge()
{:#methods:showbadge} 

To show the radialmenu item’s badge by its index

N> You can show only the already hidden badge by “hideBadge()” method.

#### Example

{% highlight html %}


       <div>
        <br />
        Click the button to hide badge value of item in index 3 <button data-role="ejmbutton" data-ej-touchend="hideBadge">Hide Badge</button><br />
        Click the button to show badge value of item in index 3 <button data-role="ejmbutton" data-ej-touchend="showBadge">Show Badge</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-imagename="social.png" data-ej-badge-value="10" data-ej-badge-enabled="true" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="social"></li>
            <li data-ej-imagename="music.png" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="music"></li>
            <li data-ej-imagename="direction.png" data-ej-badge-value="33" data-ej-badge-enabled="true" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="direction"></li>
            <li data-ej-imagename="message.png" data-ej-badge-value="5" data-ej-badge-enabled="true" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="message"></li>
            <li data-ej-imagename="browser.png" data-ej-imagepath="themes/sample/radialmenu"
                data-ej-windows-text="browser"></li>
        </ul>
    </div>

    <script>
        function hideBadge() {
            $("#defaultradialmenu").ejmRadialMenu("hideBadge", 3)
        }

        function showBadge() {
            $("#defaultradialmenu").ejmRadialMenu("showBadge", 3)
        }
    </script>


{% endhighlight %}



### showMenu()
{:#methods:showmenu} 

To Show the radialmenu when the target clicked

#### Example

{% highlight html %}


    <div>
        <br />
        <button data-role="ejmbutton" data-ej-touchend="show">Show RadialMenu</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function show() {
            $("#defaultradialmenu").ejmRadialMenu("showMenu");
        }
    </script>


{% endhighlight %}



### updateBadgeValue()
{:#methods:updatebadgevalue} 

To update badge the radialmenu item. Parameters must be passed are: 1. index of item, 2. new value

#### Example

{% highlight html %}


    <div>
        <br />
        Click the button to update badge value to 55 of item in index 2
        <button data-role="ejmbutton" data-ej-touchend="updateBadge">Update Badge</button>
    </div>
    <div id="defaultradialmenu" data-role="ejmradialmenu">
        <ul>
            <li data-ej-windows-text="google" data-ej-badge-enabled="true" data-ej-badge-value="2" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
            <li data-ej-windows-text="music" data-ej-badge-enabled="true" data-ej-badge-value="20" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
            <li data-ej-windows-text="direction" data-ej-badge-enabled="true" data-ej-badge-value="6" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
            <li data-ej-windows-text="message" data-ej-badge-enabled="true" data-ej-badge-value="10" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
            <li data-ej-windows-text="browser" data-ej-badge-enabled="true" data-ej-badge-value="15" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
        </ul>
    </div>

    <script>
        function updateBadge() {
            $("#defaultradialmenu").ejmRadialMenu("updateBadgeValue", 2, 55)
        }
    </script>




{% endhighlight %}


## Events

### close
{:#events:close} 

Event triggers while RadialMenu closing.

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
Event parameters from Radialmenu<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the Radialmenu model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
   <div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-close="close">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>

    <script>
        function close(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
 <div id="defaultradialmenu">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>
    <script>
        $("#defaultradialmenu").ejmRadialMenu({ close: "close" });

        function close(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### open
{:#events:open} 

Event triggers while RadialMenu opening.

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
Event parameters from Radialmenu<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the Radialmenu model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
<div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-open="open">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>

    <script>
        function open(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
<div id="defaultradialmenu">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>
    <script>
        $("#defaultradialmenu").ejmRadialMenu({ open: "open" });

        function open(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



### select
{:#events:select} 

[deprecated] Event triggers when we select an item.

N> Since this event deprecated, use touch event.

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
Event parameters from Radialmenu<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the Radialmenu model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
childIndex</td><td>
number</td><td>
Returns the index of selected child item</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Returns the index of selected item</td></tr>
</table>


</td></tr>
</table>

#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
<div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-select="select">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>
    <script>
        function select(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
<div id="defaultradialmenu">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>

    <script>
        $("#defaultradialmenu").ejmRadialMenu({ select: "select" });

        function select(args) {
            //handle the event
        }
    </script>




{% endhighlight %}



### touch
{:#events:touch} 

Event triggers when the touch happens.

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
Event parameters from Radialmenu<table><br><tr><br><th><b>Name</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
if the event should be canceled; otherwise, false.</td></tr>
<tr>
<td>
model</td><td>
Object</td><td>
Returns the Radialmenu model</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Returns the name of the event</td></tr>
<tr>
<td>
index </td><td>
number</td><td>
Returns the index of selected item </td></tr>
<tr>
<td>
childIndex</td><td>
number</td><td>
Returns the index of selected child item</td></tr>
</table>


</td></tr>
</table>


#### Example

{% highlight html %}


    <!-- Unobtrusive way of rendering -->
<div id="defaultradialmenu" data-role="ejmradialmenu" data-ej-touch="touch">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>

    <script>
        function touch(args) {
            //handle the event
        }
    </script>



{% endhighlight %}



{% highlight html %}


    <!-- Obtrusive way of rendering -->
<div id="defaultradialmenu">
  <ul>
      <li data-ej-windows-text="google" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/google.png"></li>
      <li data-ej-windows-text="music" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/music.png"></li>
      <li data-ej-windows-text="direction" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/direction.png"></li>
      <li data-ej-windows-text="message" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/message.png"></li>
      <li data-ej-windows-text="browser" data-ej-imageurl="http://js.syncfusion.com/UG/Mobile/Content/radial/browser.png"></li>
   </ul>      
</div>

    <script>
        $("#defaultradialmenu").ejmRadialMenu({ touch: "touch" });

        function touch(args) {
            //handle the event
        }
    </script>



{% endhighlight %}





