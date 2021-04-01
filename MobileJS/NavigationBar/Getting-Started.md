---
layout: post
title: Getting Started | Toolbar | Mobilejs | Syncfusion
description: getting started
platform: Mobilejs
control: Toolbar, NavigationBar, Header, Footer (Mobile)
documentation: ug
---

# Getting Started

## Create your first Toolbar in JavaScript

The Essential JavaScript mobile Toolbar provides a single interface to select a command from a collection of commands. It also provides template support. In this example, you can learn how to create a Mail App and through that you can learn the features of Mobile Toolbar Widget.

The Toolbar can also be Mentioned as NavigationBar,Header and Footer.

![](Getting-Started_images/Getting-Started_img1.png)

## Create the necessary layout

The Essential JavaScript Mobile Toolbar Widget is created by using number of <ul> and <li>. Each <li> item performs individual actions. You can customize the Toolbar control by changing its properties according to your requirement. In this scenario, a _back_ toolbar item is used to navigate to previous page, _next_ toolbar item to show the next email in the inbox, _compose_ toolbar item to compose new mail, delete toolbar item to delete current mail, and close toolbar item to close the inbox app. The following steps guide you in creating a basic Toolbar for your application.

Create an HTML file and add the following template to the html file for Toolbar creation.

{% highlight html %}

<!DOCTYPE html>

<html>

	<head>

		<title>Toolbar</title>

		<link href="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.css" rel="stylesheet" />

		<script src="http://cdn.syncfusion.com/js/assets/external/jquery-3.0.0.min.js"></script>
		<script src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
		<script src="http://cdn.syncfusion.com/js/assets/external/jquery.globalize.min.js"></script>
		<script src="http://cdn.syncfusion.com/{{ site.releaseversion }}/js/mobile/ej.mobile.all.min.js"></script>
	</head>

	<body>
		<div class="default splitpane control">
      	  <div id="defaultsplitpane" data-role="ejmsplitpane"  data-ej-contentpane-templateid="splitpanecontentPane" data-ej-leftpane-showontablet="false">
      	  </div>
       	 <script id="splitpanecontentPane" type="text/x-jsrender">
         	   <div id="splitHeader" data-role="ejmnavigationbar" data-ej-mode="header">
                <button data-ej-cssclass="e-m-left" id="openDrawer" data-role="ejmactionlink" data-ej-contenttype="image" data-ej-showborder="false" data-ej-imageclass="nav-icon e-m-sbicon-drawermenu" data-ej-touchend="onNavOpen"></button>
                <span id="mailHeadText" class="e-m-navbar-text e-m-title-left" style="margin-left: 48px;">Inbox</span>
            	</div>        
         </script>
   		</div>
		
	</body>

</html>

{% endhighlight %}

Add the following code in your style section to use font icons in your sample,

{% highlight css %}

	<style>
	
    @font-face {
    font-family: 'ejmsbfonts';
    src: url('../themes/sbimages/ejmsbfonts.eot?rzt8lw');
    src: url('../themes/sbimages/ejmsbfonts.eot?rzt8lw#iefix') format('embedded-opentype'), url('../themes/sbimages/ejmsbfonts.ttf?rzt8lw') format('truetype'), url('../themes/sbimages/ejmsbfonts.woff?rzt8lw') format('woff'), url('../themes/sbimages/ejmsbfonts.svg?rzt8lw#ejmsbfonts') format('svg');
    font-weight: normal;
    font-style: normal;
    }
	
	.e-m-sbicon-drawermenu{
    font-family: 'ejmsbfonts' !important;
	}
	
   .e-m-sbicon-drawermenu:before {
    content: "\e93e";
    }

	</style>

{% endhighlight %}

Execute this code to render the following output.

![](Getting-Started_images/Getting-Started_img2.png)

### Adding ListView in NavigationBar

You can render required control in the NavigationBar. The below example shows you how to use ejmListView in slider panel.

Add following code in your html page,

{% highlight html %}

	<div class="default splitpane control">
        <div id="defaultsplitpane" data-role="ejmsplitpane" data-ej-leftpane-templateid="splitpaneleftPane" data-ej-contentpane-templateid="splitpanecontentPane" data-ej-leftpane-showontablet="false">
        </div>
        <script id="splitpaneleftPane" type="text/x-jsrender">
            <div id="leftHeader" data-role="ejmnavigationbar" style="height:130px;">
                <div id="userimg">
                </div>
                <div id="username">
                    Orville M. Brown
                </div>
            </div>
            <div id="navLeftScroll" data-role="ejmscrollpanel" style="top:130px;">
                <div id="listLeftPane" data-role="ejmlistview" data-ej-selectedindex="0" data-ej-touchend="_optionClick" data-ej-persistselection="true" data-ej-datasource="window.optionList" data-ej-templateid="optionList">
                </div>
            </div>
        </script>
        <script id="splitpanecontentPane" type="text/x-jsrender">
            <div id="splitHeader" data-role="ejmnavigationbar" data-ej-mode="header">
                <button data-ej-cssclass="e-m-left" id="openDrawer" data-role="ejmactionlink" data-ej-contenttype="image" data-ej-showborder="false" data-ej-imageclass="nav-icon e-m-sbicon-drawermenu" data-ej-touchend="onNavOpen"></button>
                <span id="mailHeadText" class="e-m-navbar-text e-m-title-left" style="margin-left: 48px;">Inbox</span>
            </div>
            <div id="navContentScroll" data-role="ejmscrollpanel">
                <div id="list" data-role="ejmlistview" data-ej-preventselection="true" data-ej-datasource="window.listData" data-ej-templateid="emailList">
                </div>
            </div>
        </script>
        <script id="emailList" type="text/x-jsrender">
            <span class="item-lst">
                <div class="cnt">
                    <span class="lst-ima">
                        <img src="themes/sampleimages/splitpane/{{>class}}.png" class="img-{{>class}} user-image" />
                    </span>
            <span class='lst-content'>
                        <span class="lst-name">{{>name}}</span>
            <span class="lst-time">{{>time}}</span>
            <span class="lst-sub">{{>subject}}</span>
            <span class="lst-des">{{>description}}</span>
            </span>
    </div>
    </span>
    </script>

    <script id="optionList" type="text/x-jsrender">
        <span class="opt-lst">
                <span class="opt-img">
                    <img src="themes/sampleimages/splitpane/icons/{{>icon}}.png" class="img-{{>icon}} user-image" />
                </span>
        <span class='opt-content'>
                    <span class="opt-name">{{>text}}</span>
        </span>
        </span>
    </script>
    </div>

{% endhighlight %}

Add the following code in your script section,

{% highlight javascript %}

function _optionClick(e) {
            switch (e.data.text) {
            case "Inbox":
                $("#list").ejmListView("option", "dataSource", window.listData);
                break;
            case "Sent Item":
                $("#list").ejmListView("option", "dataSource", window.sentItemData);
                break;
            case "Outbox":
                $("#list").ejmListView("option", "dataSource", window.outboxData);
                break;
            }
            $("#mailHeadText").text(e.data.text);
            $("#defaultsplitpane").ejmSplitPane("closePane");
            $("#navContentScroll").ejmScrollPanel("scrollTo",0,0);
        }

        function onNavOpen() {
            $("#defaultsplitpane").ejmSplitPane("openLeftPane");

        }
	
	{% endhighlight %}

	Some time if you don't want to refer entire css file, please refer the icons as individual by using the below code in style section,

	{% highlight css %}

	@font-face {
    font-family: 'ejmsbfonts';
    src: url('../themes/sbimages/ejmsbfonts.eot?rzt8lw');
    src: url('../themes/sbimages/ejmsbfonts.eot?rzt8lw#iefix') format('embedded-opentype'), url('../themes/sbimages/ejmsbfonts.ttf?rzt8lw') format('truetype'), url('../themes/sbimages/ejmsbfonts.woff?rzt8lw') format('woff'), url('../themes/sbimages/ejmsbfonts.svg?rzt8lw#ejmsbfonts') format('svg');
    font-weight: normal;
    font-style: normal;
    }
	
	.e-m-sbicon-drawermenu{
    font-family: 'ejmsbfonts' !important;
	}
	
   .e-m-sbicon-drawermenu:before {
    content: "\e93e";
    }

	{% endhighlight %}

Execute the above mentioned code to get following output.

![](Getting-Started_images/Getting-Started_img1.png)