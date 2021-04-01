---
layout: post
title: Header Postioning | Header | Mobilejs | Syncfusion
description: header templateid
platform: Mobilejs
control: Toolbar, NavigationBar, Header, Footer(Mobile)
documentation: ug
keywords: position
---

# Header positioning

data-ej-position is used to change the position.The default value of position is top.

The position type is

* Top

* Bottom

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
            <div id="splitHeader" data-role="ejmnavigationbar" data-ej-mode="header" data-ej-title="Inbox" data-ej-titlealignment="center" data-ej-position="bottom" >
                <button data-ej-cssclass="e-m-left" id="openDrawer" data-role="ejmactionlink" data-ej-contenttype="image" data-ej-showborder="false" data-ej-imageclass="nav-icon e-m-sbicon-drawermenu" data-ej-touchend="onNavOpen"></button>
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
                        <img src="../themes/sampleimages/splitpane/{{>class}}.png" class="img-{{>class}} user-image" />
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
                    <img src="../themes/sampleimages/splitpane/icons/{{>icon}}.png" class="img-{{>icon}} user-image" />
                </span>
        <span class='opt-content'>
                    <span class="opt-name">{{>text}}</span>
        </span>
        </span>
    </script>

    <script>
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
    </script>
    </div>

{% endhighlight %}

Execute the above mentioned code to get following output.

![](Header-Positioning-images/header-positioning-img1.png)