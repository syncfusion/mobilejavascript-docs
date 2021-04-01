---
layout: post
title: Getting-Started | SplitPane | Mobilejs | Syncfusion
description: getting started
platform: js
control: SplitPane (Mobile)
documentation: ug
---

# Getting started

This section enables you to create **SplitPane** using JavaScript in your mobile app.

The **SplitPane** can be easily configured to the div element in which the **SplitPane** is placed in one main div. The **SplitPane** consists of three div’s for following purpose 

1. Left Pane layout

2. Content Pane Layout

3. Right Pane Layout

From the following guidelines, you can learn about the features in mobile **SplitPane** widget by creating a Mail App. The following screenshot demonstrates the functionality of **SplitPane** widget.




![getting-started](getting-started_images\getting-started_img1.png)

## Creating basic mobile layout

The **Essential JavaScript Mobile Splitpane** widget is rendered based on the default values for all the properties. You can easily customize the **SplitPane** control by changing their properties according to your need. The following steps guide you to create a Mail App.

Create an **HTML** file and paste the following template to it for Mail App creation.

{% highlight html %}

<!DOCTYPE html>
<html>
<head>
    <title>Splitpane</title>
<link href="http://cdn.syncfusion.com/14.3.0.49/js/mobile/ej.mobile.all.min.css"rel="stylesheet"/>
<script src="http://cdn.syncfusion.com/js/assets/external/jquery-1.10.2.min.js"></script>
<script src="http://cdn.syncfusion.com/js/assets/external/jsrender.min.js"></script>
<script src="http://cdn.syncfusion.com/14.3.0.49/js/mobile/ej.mobile.all.min.js"></script>
</head>
<body>
                <!--Add Splitpane Element here-->
</body>
</html>



{% endhighlight %}

## Create a SplitPane control

To render the **SplitPane** control, you need to set `data-role` attribute to `ejmsplitpane` to a div element. 

Refer the following code example.

{% highlight html %}

<div id="defaultsplitpane" data-role="ejmsplitpane">
        <div data-ej-pane="left" id="leftPane">
            <!--Left pane content-->	
        </div>
        <div data-ej-pane="content" id="contentPane">
            <!--Content pane content-->	
        </div>
    </div>


{% endhighlight %}



## Add pane content

To set left pane or right pane header title by **Navigationbar** control with the desired template content, set it as user profile. Use **ListView** control with template support to display the left pane or right pane content.



To set content pane header title by **Navigationbar** control with the desired title, set it as Inbox. Use **ListView** control with template support to display the content pane’s content. When you click the left pane or right pane list item, you can update the content pane content through **ListView** by setting the dataSource to it. The left pane or right pane list item selection is handled by **listItemSelect** function.

### Left pane configuration

The `data-ej-leftpane-showontablet` attribute is used to specifies the leftpane visibility for tablet devices. If this property set as false, the leftpane will be hidden and it will be open from left side window on swipe.



Refer to the following code example.
{% tabs %}
{% highlight html %}


<div class="default splitpane control">
        <div id="defaultsplitpane" data-role="ejmsplitpane" data-ej-leftpane-showontablet="true">
            <div data-ej-pane="left" id="leftPane">
                <div id="leftHeader" data-role="ejmnavigationbar" style="height:130px;">
                    <div id="userimg">
                    </div>
                    <div id="username">
                        Orville M. Brown
                    </div>
                </div>
                <div id="navLeftScroll" data-role="ejmscrollpanel" style="top:130px;">
                    <div id="listLeftPane" data-role="ejmlistview" data-ej-selectedindex="0" data-ej-touchend="listItemSelect" data-ej-persistselection="true" data-ej-datasource="window.optionList" data-ej-templateid="optionList">
                    </div>
                </div>
            </div>
            <div data-ej-pane="content" id="contentPane">
                <div id="splitHeader" data-role="ejmnavigationbar" data-ej-mode="header">
                    <span id="mailHeadText" class="e-m-navbar-text e-m-title-left" style="margin-left: 20px;">Inbox</span>
                </div>
                <div id="navContentScroll" data-role="ejmscrollpanel">
                    <div id="list" data-role="ejmlistview" data-ej-preventselection="true" data-ej-datasource="window.listData" data-ej-templateid="emailList">
                    </div>
                </div>
            </div>

        </div>
        <script id="emailList" type="text/x-jsrender">
            <span class="item-lst">
                <div class="cnt">
                    <span class="lst-ima">
                        <img src="../themes/sampleimages/splitpane/**{{>class}}**.png" class="img-**{{>class}}** user-image" />
                    </span>
                    <span class='lst-content'>
                        <span class="lst-name">**{{>name}}**</span>
                        <span class="lst-time">**{{>time}}**</span>
                        <span class="lst-sub">**{{>subject}}**</span>
                        <span class="lst-des">**{{>description}}**</span>
                    </span>
                </div>
            </span>
        </script>

        <script id="optionList" type="text/x-jsrender">
            <span class="opt-lst">
                <span class="opt-img">
                    <img src="../themes/sampleimages/splitpane/icons/**{{>icon}}**.png" class="img-**{{>icon}}** user-image" />
                </span>
                <span class='opt-content'>
                    <span class="opt-name">**{{>text}}**</span>
                </span>
            </span>
        </script>


{% endhighlight %}



{% highlight js %}



        // data source for listbox with right pane’s url for each item

  window.listData = [{
                "name": "Frank M. Eisele ",
                "class": "brooke",
                "time": "10:15 AM",
                "subject": "Weekend Trip Plan",
                "description": "Hi, Please have a pre look what are all place gonna visit."
            },
             {
                 "name": "Kendra M. Price",
                 "class": "claire",
                 "time": "12:00 PM",
                 "subject": "Re : David Party",
                 "description": "Can we go to the party by 9 O'Clk Get ready."
             },
             {
                 "name": "Adele D. Schreffler",
                 "class": "erik",
                 "time": "1:06 PM",
                 "subject": "Meeting Appoinment",
                 "description": "Hi Schreffler, We have scheduled meeting for our discussion."
             },
             {
                 "name": "Ellen A. Deeds",
                 "class": "grace",
                 "time": "2:11 PM",
                 "subject": "Fw : Critical Update",
                 "description": "Deeds, Please receive the critical from the host."
             },
            ];

            window.optionList = [
            { icon: "inbox", text: "Inbox" },
            { icon: "sent", text: "Sent Item" },
            { icon: "outbox", text: "Outbox" }
            ];

            window.sentItemData = [

                {
                    "name": "David J. Thomas",
                    "class": "jacob",
                    "time": "4:03 PM",
                    "subject": "Re : Home Page Design",
                    "description": "I applied those updates, here's the latest design for the homepage."
                },
                {
                    "name": "Harriett T. Jolley",
                    "class": "claire",
                    "time": "12:00 PM",
                    "subject": "Re : David Party",
                    "description": "Can we go to the party by 9 O'Clk Get ready."
                },
                {
                    "name": "Andrew M. Yager",
                    "class": "erik",
                    "time": "1:06 PM",
                    "subject": "Fw : Meeting Appoinment",
                    "description": "Hi Yager, We have scheduled meeting for our discussion."
                }
            ];

            window.outboxData = [
                {
                    "name": "Frank M. Eisele ",
                    "class": "brooke",
                    "time": "10:15 AM",
                    "subject": "Weekend Trip Plan",
                    "description": "Hi, Please have a pre look what are all place gonna visit."
                },
                {
                    "name": "Kendra M. Price",
                    "class": "claire",
                    "time": "12:00 PM",
                    "subject": "Re : David Party",
                    "description": "Can we go to the party by 9 O'Clk Get ready."
                },
                {
                    "name": "Adele D. Schreffler",
                    "class": "erik",
                    "time": "1:06 PM",
                    "subject": "Meeting Appoinment",
                    "description": "Hi Schreffler, We have scheduled meeting for our discussion."
                },
                {
                    "name": "Harriett T. Jolley",
                    "class": "claire",
                    "time": "12:00 PM",
                    "subject": "Re : David Party",
                    "description": "Can we go to the party by 9 O'Clk Get ready."
                }];
            function listItemSelect (e) {
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
                $("#navContentScroll").ejmScrollPanel("scrollTo", 0, 0);
            }

            function onNavOpen() {
                $("#defaultsplitpane").ejmSplitPane("openLeftPane");

            }   


{% endhighlight %}

{% highlight css %}


          .default.splitpane #userimg {
            background-image: url("../themes/sampleimages/splitpane/brooke.png");
            background-position: center top;
            background-repeat: no-repeat;
            background-size: 100% 100%;
            border: 1px solid #ccc;
            border-radius: 50%;
            height: 80px;
            margin: 0 auto;
            width: 80px;
        }

        .default.splitpane #username {
            margin-top: 10px;
            width: 100%;
            text-align: center;
            text-transform: uppercase;
            font-weight: 600;
        }

        .default.splitpane #list .e-m-lv {
            background-color: white;
        }

        .default.splitpane #list .e-m-lv-item {
            border-bottom: 1px solid #a5a5a5;
            padding: 5px 0px;
        }

        .default.splitpane #splitHeader .e-m-navbar-text {
            letter-spacing: 2px;
            font-weight: 600;
            font-family: sans-serif;
        }

        .default.splitpane .lst-time {
            color: darkblue;
            position: absolute;
            right: 8px;
            top: 5px;
        }

        .default.splitpane .e-m-lv-active .item-lst {
            color: #fff;
        }

        .default.splitpane .item-lst {
            color: #333;
            display: block;
            font-family: Helvetica Neue, Helvetica;
            font-size: 14px;
            min-height: 68px;
            position: relative;
        }

         .default.splitpane .item-lst span {
                display: block;
            }

        .default.splitpane .lst-ima {
            bottom: 0;
            left: 0;
            position: absolute;
            top: 5;
            width: 65px;
        }

        .default.splitpane .lst-content {
            bottom: 0;
            left: 66px;
            position: absolute;
            right: 0;
            top: 0;
        }

        .default.splitpane .lst-name {
            font-size: 16px;
            font-weight: bold;
            margin-top: 5px;
        }

        .default.splitpane .lst-des {
            font-size: 12px;
            margin-top: 3px;
            text-overflow: ellipsis;
            padding-right: 10px;
            white-space: nowrap;
            overflow: hidden;
        }

        .default.splitpane .lst-sub {
            font-size: 13px;
            font-weight: bold;
            margin-top: 7px;
        }

        .default.splitpane .opt-img {
            width: 38px;
            left: 0;
        }

        .default.splitpane .opt-lst {
            height: 47px;
            display: block;
            border-bottom: 1px solid #ccc;
            padding-top: 5px;
            font-family: sans-serif;
            font-size: 16px;
            font-weight: 600;
        }

            .default.splitpane .opt-lst span {
                display: block;
                color: #333;
                letter-spacing: 1px;
            }

        .default.splitpane .e-m-lv-active .opt-lst span {
            color: #fff;
        }

        .default.splitpane .opt-name {
            padding-top: 10px;
        }

        .default.splitpane .opt-content {
            position: absolute;
            left: 36px;
            right: 0;
            top: 0;
            bottom: 0;
            padding: 5px;
        }

        .default.splitpane .opt-img img {
            background-repeat: no-repeat;
            bottom: 7px;
            display: block;
            height: 51px;
            padding: 7px;
            position: relative;
            width: 45px;
        }

        .default.splitpane #contentscroll {
            background: #fff;
        }


        .default.splitpane .nav-icon::before {
            font-size: 22px;
        }

        .default.splitpane .e-m-windows.nav-icon::before {
            color: #000;
        }

        default.splitpane .e-m-android.nav-icon {
            position: absolute;
            left: 4px;
            top: 13px;
        }

        .default.splitpane .e-m-windows.nav-icon, .default.splitpane .e-m-flat.nav-icon {
            position: absolute;
            left: 5px;
        }

        .default.splitpane .e-m-flat.nav-icon {
            top: 11px;
        }

        .default.splitpane .e-m-android.nav-icon::before {
            color: #fff;
            font-size: 32px;
        }

        .default.splitpane .e-m-flat.nav-icon::before {
            color: #fff;
        }

        .default.splitpane .e-m-ios7.nav-icon::before {
            color: #2883f2;
        }

        .default.splitpane .e-m-ios7.nav-icon {
            position: absolute;
            left: 6px;
            top: 6px;
        }


{% endhighlight %}
{% endtabs %}


Run this code and you can see the following output.

![LeftPane-Content](getting-started_images\getting-started_img2.png)


### Right pane configuration

The `data-ej-rightpane-showontablet` attribute is used to specifies the rightpane visibility for tablet devices. If this property set as false, the rightpane will be hidden and it will be open from right side window on swipe.



Refer to the following code example.

{% tabs %}
{% highlight html %}


<div class="default splitpane control">
        <div id="defaultsplitpane" data-role="ejmsplitpane" data-ej-rightpane-showontablet="true">
            <div data-ej-pane="right" id="rightPane">
                <div id="rightHeader" data-role="ejmnavigationbar" style="height:130px;">
                    <div id="userimg">
                    </div>
                    <div id="username">
                        Orville M. Brown
                    </div>
                </div>
                <div id="navLeftScroll" data-role="ejmscrollpanel" style="top:130px;">
                    <div id="listLeftPane" data-role="ejmlistview" data-ej-selectedindex="0" data-ej-touchend="listItemSelect" data-ej-persistselection="true" data-ej-datasource="window.optionList" data-ej-templateid="optionList">
                    </div>
                </div>
            </div>
            <div data-ej-pane="content" id="contentPane">
                <div id="splitHeader" data-role="ejmnavigationbar" data-ej-mode="header">
                    <span id="mailHeadText" class="e-m-navbar-text e-m-title-left" style="margin-left: 20px;">Inbox</span>
                </div>
                <div id="navContentScroll" data-role="ejmscrollpanel">
                    <div id="list" data-role="ejmlistview" data-ej-preventselection="true" data-ej-datasource="window.listData" data-ej-templateid="emailList">
                    </div>
                </div>
            </div>

        </div>
        <script id="emailList" type="text/x-jsrender">
            <span class="item-lst">
                <div class="cnt">
                    <span class="lst-ima">
                        <img src="../themes/sampleimages/splitpane/**{{>class}}**.png" class="img-**{{>class}}** user-image" />
                    </span>
                    <span class='lst-content'>
                        <span class="lst-name">**{{>name}}**</span>
                        <span class="lst-time">**{{>time}}**</span>
                        <span class="lst-sub">**{{>subject}}**</span>
                        <span class="lst-des">**{{>description}}**</span>
                    </span>
                </div>
            </span>
        </script>

        <script id="optionList" type="text/x-jsrender">
            <span class="opt-lst">
                <span class="opt-img">
                    <img src="../themes/sampleimages/splitpane/icons/**{{>icon}}**.png" class="img-**{{>icon}}** user-image" />
                </span>
                <span class='opt-content'>
                    <span class="opt-name">**{{>text}}**</span>
                </span>
            </span>
        </script>


{% endhighlight %}

{% highlight js %}



        // data source for listbox with right pane’s url for each item

  window.listData = [{
                "name": "Frank M. Eisele ",
                "class": "brooke",
                "time": "10:15 AM",
                "subject": "Weekend Trip Plan",
                "description": "Hi, Please have a pre look what are all place gonna visit."
            },
             {
                 "name": "Kendra M. Price",
                 "class": "claire",
                 "time": "12:00 PM",
                 "subject": "Re : David Party",
                 "description": "Can we go to the party by 9 O'Clk Get ready."
             },
             {
                 "name": "Adele D. Schreffler",
                 "class": "erik",
                 "time": "1:06 PM",
                 "subject": "Meeting Appoinment",
                 "description": "Hi Schreffler, We have scheduled meeting for our discussion."
             },
             {
                 "name": "Ellen A. Deeds",
                 "class": "grace",
                 "time": "2:11 PM",
                 "subject": "Fw : Critical Update",
                 "description": "Deeds, Please receive the critical from the host."
             },
            ];

            window.optionList = [
            { icon: "inbox", text: "Inbox" },
            { icon: "sent", text: "Sent Item" },
            { icon: "outbox", text: "Outbox" }
            ];

            window.sentItemData = [

                {
                    "name": "David J. Thomas",
                    "class": "jacob",
                    "time": "4:03 PM",
                    "subject": "Re : Home Page Design",
                    "description": "I applied those updates, here's the latest design for the homepage."
                },
                {
                    "name": "Harriett T. Jolley",
                    "class": "claire",
                    "time": "12:00 PM",
                    "subject": "Re : David Party",
                    "description": "Can we go to the party by 9 O'Clk Get ready."
                },
                {
                    "name": "Andrew M. Yager",
                    "class": "erik",
                    "time": "1:06 PM",
                    "subject": "Fw : Meeting Appoinment",
                    "description": "Hi Yager, We have scheduled meeting for our discussion."
                }
            ];

            window.outboxData = [
                {
                    "name": "Frank M. Eisele ",
                    "class": "brooke",
                    "time": "10:15 AM",
                    "subject": "Weekend Trip Plan",
                    "description": "Hi, Please have a pre look what are all place gonna visit."
                },
                {
                    "name": "Kendra M. Price",
                    "class": "claire",
                    "time": "12:00 PM",
                    "subject": "Re : David Party",
                    "description": "Can we go to the party by 9 O'Clk Get ready."
                },
                {
                    "name": "Adele D. Schreffler",
                    "class": "erik",
                    "time": "1:06 PM",
                    "subject": "Meeting Appoinment",
                    "description": "Hi Schreffler, We have scheduled meeting for our discussion."
                },
                {
                    "name": "Harriett T. Jolley",
                    "class": "claire",
                    "time": "12:00 PM",
                    "subject": "Re : David Party",
                    "description": "Can we go to the party by 9 O'Clk Get ready."
                }];
            function listItemSelect (e) {
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
                $("#navContentScroll").ejmScrollPanel("scrollTo", 0, 0);
            }

            function onNavOpen() {
                $("#defaultsplitpane").ejmSplitPane("openLeftPane");

            }   


{% endhighlight %}

{% highlight css %}


          .default.splitpane #userimg {
            background-image: url("../themes/sampleimages/splitpane/brooke.png");
            background-position: center top;
            background-repeat: no-repeat;
            background-size: 100% 100%;
            border: 1px solid #ccc;
            border-radius: 50%;
            height: 80px;
            margin: 0 auto;
            width: 80px;
        }

        .default.splitpane #username {
            margin-top: 10px;
            width: 100%;
            text-align: center;
            text-transform: uppercase;
            font-weight: 600;
        }

        .default.splitpane #list .e-m-lv {
            background-color: white;
        }

        .default.splitpane #list .e-m-lv-item {
            border-bottom: 1px solid #a5a5a5;
            padding: 5px 0px;
        }

        .default.splitpane #splitHeader .e-m-navbar-text {
            letter-spacing: 2px;
            font-weight: 600;
            font-family: sans-serif;
        }

        .default.splitpane .lst-time {
            color: darkblue;
            position: absolute;
            right: 8px;
            top: 5px;
        }

        .default.splitpane .e-m-lv-active .item-lst {
            color: #fff;
        }

        .default.splitpane .item-lst {
            color: #333;
            display: block;
            font-family: Helvetica Neue, Helvetica;
            font-size: 14px;
            min-height: 68px;
            position: relative;
        }

         .default.splitpane .item-lst span {
                display: block;
            }

        .default.splitpane .lst-ima {
            bottom: 0;
            left: 0;
            position: absolute;
            top: 5;
            width: 65px;
        }

        .default.splitpane .lst-content {
            bottom: 0;
            left: 66px;
            position: absolute;
            right: 0;
            top: 0;
        }

        .default.splitpane .lst-name {
            font-size: 16px;
            font-weight: bold;
            margin-top: 5px;
        }

        .default.splitpane .lst-des {
            font-size: 12px;
            margin-top: 3px;
            text-overflow: ellipsis;
            padding-right: 10px;
            white-space: nowrap;
            overflow: hidden;
        }

        .default.splitpane .lst-sub {
            font-size: 13px;
            font-weight: bold;
            margin-top: 7px;
        }

        .default.splitpane .opt-img {
            width: 38px;
            left: 0;
        }

        .default.splitpane .opt-lst {
            height: 47px;
            display: block;
            border-bottom: 1px solid #ccc;
            padding-top: 5px;
            font-family: sans-serif;
            font-size: 16px;
            font-weight: 600;
        }

            .default.splitpane .opt-lst span {
                display: block;
                color: #333;
                letter-spacing: 1px;
            }

        .default.splitpane .e-m-lv-active .opt-lst span {
            color: #fff;
        }

        .default.splitpane .opt-name {
            padding-top: 10px;
        }

        .default.splitpane .opt-content {
            position: absolute;
            left: 36px;
            right: 0;
            top: 0;
            bottom: 0;
            padding: 5px;
        }

        .default.splitpane .opt-img img {
            background-repeat: no-repeat;
            bottom: 7px;
            display: block;
            height: 51px;
            padding: 7px;
            position: relative;
            width: 45px;
        }

        .default.splitpane #contentscroll {
            background: #fff;
        }


        .default.splitpane .nav-icon::before {
            font-size: 22px;
        }

        .default.splitpane .e-m-windows.nav-icon::before {
            color: #000;
        }

        default.splitpane .e-m-android.nav-icon {
            position: absolute;
            left: 4px;
            top: 13px;
        }

        .default.splitpane .e-m-windows.nav-icon, .default.splitpane .e-m-flat.nav-icon {
            position: absolute;
            left: 5px;
        }

        .default.splitpane .e-m-flat.nav-icon {
            top: 11px;
        }

        .default.splitpane .e-m-android.nav-icon::before {
            color: #fff;
            font-size: 32px;
        }

        .default.splitpane .e-m-flat.nav-icon::before {
            color: #fff;
        }

        .default.splitpane .e-m-ios7.nav-icon::before {
            color: #2883f2;
        }

        .default.splitpane .e-m-ios7.nav-icon {
            position: absolute;
            left: 6px;
            top: 6px;
        }


{% endhighlight %}
{% endtabs %}


Run this code and you can see the following output.



![RightPane-Content](getting-started_images\getting-started_img3.png)

