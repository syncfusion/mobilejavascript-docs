---
layout: post
title: Header TemplateId | Header | Mobilejs | Syncfusion
description: header templateid
platform: Mobilejs
control: Toolbar, NavigationBar, Header, Footer (Mobile)
documentation: ug
keywords: template
---

# Header templateid

data-ej-templateid is used to define the ID of the template element where you can specify the content to render in the control. The below code is used to rendered ejmlistview as template in the NavigationBar.

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
		</div>

{% endhighlight %}

Execute the above mentioned code to get following output.

![](Header-TemplateId_images/Header-TemplateId_img1.png)