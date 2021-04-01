---
layout: post
title: Getting Started | Button | Mobilejs | Syncfusion
description: getting started
platform: Mobilejs
control: Button (Mobile)
documentation: ug
---

# Getting Started

## Create your first Menu in JavaScript

From the following guidelines, you can create a Media Player App where you can learn the mobile button features.

The following screenshot illustrates the functionality of a Button control in Media Player.

![](Getting-Started_images/Getting-Started_img1.jpg)

### Create the necessary layout

Create an HTML file and paste the following template to it for Button creation.

{% highlight html %}

    <!DOCTYPE html>
    <html>
    <head>
        <meta id="viewport" name="viewport" content="width=device-width, initial-scale=1.0,maximum-scale=1.0, user-scalable=no" />
        <title>Button</title>
        <link rel="stylesheet" href="http://cdn.syncfusion.com/14.3.0.49/js/mobile/ej.mobile.all.min.css" />
        <script type="text/javascript" src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>
        <script type="text/javascript" src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
        <script type="text/javascript" src="http://cdn.syncfusion.com/14.3.0.49/js/mobile/ej.mobile.all.min.js"></script>
        <!--Add custom scripts here -->
    </head>
    <body>
        <div>
            <div id="header" data-role="ejmnavigationbar" data-ej-title="Audio Player" data-ej-isrelative="true" data-ej-titlealignment="center"></div>
            <div id="content">
                <div align="center" class="center">
                    <!--Mobile Button control  -->                
                </div>
            </div>
        </div>
    </body>
    </html>

{% endhighlight %}

Add the following styles to add formatting to your page.

{% highlight css %}

    .center {
    padding: 20px;
    top: 20px;
    position: relative;
    }
    td {
    padding: 10px;
    }
	   
{% endhighlight %}

You can add Audio controls in your app by using html audio control. Add the following code example inside the Div element. 

{% highlight html %}

    <!--Audio-->

    <audio controls id="audio">

        <source src="audio/song.wav" type="audio/wav">

        <source src="audio/song.ogg" type="audio/ogg">

        <source src="audio/song.mp3" type="audio/mp3">

    </audio>

    <br />
    <br />

{% endhighlight %}

N> Make sure you have an audio file in specified location.

Run the above code example to render the following output.

![](Getting-Started_images/Getting-Started_img2.jpg)


### Create Button Widget

To render the Button control, set “data-role” attribute to “ejmbutton” to an “input” element.

In your Media player, add three buttons for “Play”, “Pause” and “Save” as per the following code.

{% highlight html %}

    <table>
           <tr>
                <td>
                    <input type="button" id="play" data-role="ejmbutton" />
                </td>
                <td>
                    <input type="button" id="pause" data-role="ejmbutton" />
                </td>
                <td>
                    <input type="button" id="stop" data-role="ejmbutton" />
                </td>
           </tr>
     </table>

{% endhighlight %}

### Set text

Now, set text for all the buttons. You can achieve this by using “data-ej-text” attribute. 

{% highlight html %}

<!--Button-->

    <table>
            <tr>
                <td>
                    <input type="button" id="play" data-role="ejmbutton" data-ej-text="Play"/>
                </td>
                <td>
                    <input type="button" id="pause" data-role="ejmbutton" data-ej-text="Pause" />
                </td>
                <td>
                    <input type="button" id="stop" data-role="ejmbutton" data-ej-text="Save" />
                </td>
            </tr>
    </table>

{% endhighlight %}

![](Getting-Started_images/Getting-Started_img1.jpg)

### Saving the Audio file

Simply, a Dialog control is added to alert you when the file is saved.

For this purpose, use Mobile dialog control that can be rendered with the code example provided as follows.

{% highlight html %}

    <div id="alertdlg" data-role="ejmdialog" data-ej-title="Save" data-ej-mode="alert" data-ej-leftbuttoncaption="Ok" data-ej-enablemodal="false" data-ej-enableautoopen="false" data-ej-buttontap="alertClose">
         <div>
            Your Audio has been saved.
         </div>
    </div>

{% endhighlight %}

### Binding Events

You can bind Button controls touch events to the html audio control by using the events provided by Button Widget.

You can achieve this by using “data-ej-touchend” attribute.

{% highlight html %}

<!--Button-->

     <table>
          <tr>
              <td>
                  <input type="button" id="play" data-role="ejmbutton" data-ej-text="Play" data-ej-touchend="play" />
              </td>
              <td>
                  <input type="button" id="pause" data-role="ejmbutton" data-ej-text="Pause" data-ej-touchend="pause" />
              </td>
              <td>
                  <input type="button" id="stop" data-role="ejmbutton" data-ej-text="Save"  data-ej-touchend="save" />
              </td>
          </tr>
    </table>

{% endhighlight %}

At this point, you have created all the elements required for a simple Mediaplayer.

Next, write a code for binding button events with Audio control.

You can achieve this by using the following Script.

{% highlight js %}

var v = document.getElementsByTagName("audio")[0];

v.pause();

function play() {

	v.play();

}

function pause() {

	v.pause();

}

function save() {

	App.activePage.find("#alertdlg").ejmDialog("open");

}

function alertClose(args) {

	App.activePage.find("#alertdlg").ejmDialog("close");

}

{% endhighlight %}