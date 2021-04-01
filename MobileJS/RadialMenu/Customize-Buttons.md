---
layout: post
title: customize-buttons
description: customize buttons
platform: js
control: RadialMenu
documentation: ug
keywords: radialmenu, button, back-button
---

## Customize buttons

You can simply customize the Radial Menu Center and Back buttons (images) by using data-ej-imageclass and data-ej-backimageclass attributes respectively. 

The Radial Menu control is essentially a context menu presenting its items in a circular arrangement around a center button. Sub-Items are also supported in Radial Menu. To navigate to sub items, click the center button and the corresponding sub-items group is displayed. Nested Radial menu contains the second level back button. In this case you can use data-ej-backimageclass attribute to change the back button image. 

Refer to the following code example.

{% highlight html %}


    <div id="radialmenu_sample" data-role="ejmradialmenu" data-ej-position="leftcenter" data-ej-imageclass="imageclass" data-ej-backimageclass="backimage">
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



{% endhighlight %}

Refer the below code snippets for css class

{% highlight css %}

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


{% endhighlight %}



![](customize-buttons_images\customize-buttons_img1.png)





![](customize-buttons_images\customize-buttons_img2.png)

