---
layout: post
title: templating
description: templating
platform: js
control: ListView
documentation: ug
---

## Templating

Internal Template

By using template support, you can customize the appearance of the individual list item or render the whole ListView by using a single template. Setting the TemplateID and renders the ListView with template item.

{% highlight html %}

<div class="sample-control template listview">
        <div id="appScroll">
            <ul data-role="ejmlistview" id="templatelist" data-ej-datasource="window.dbitem" data-ej-templateid="lvtemplate"></ul>
        </div>
    </div>
    <script id="lvtemplate" type="text/x-jsrender">
        <div class="cont-bg">
            <div class="profile {{>Class}}">
            </div>
            <div class="listrightdiv">
                <span class="templatetext">{{>Name}}</span> <span class="designationstyle">{{>Designation}}</span>
                <div class="aboutstyle">
                    {{>About}}
                </div>
            </div>
        </div>
   </script>


{% endhighlight %}



{% highlight js %}

  window.dbitem =
        [{ "Name": "Brooke", "Class": "brooke", "Designation": "HR Assistant", "About": "Brooke provides administrative support to the HR office." },
        { "Name": "Claire", "Class": "claire", "Designation": "HR Manager", "About": "Claire is responsible for strategic HR planning and budget." },
        { "Name": "Erik", "Class": "erik", "Designation": "Training Specialist", "About": "Erik notifies attendees and manages follow up." },
        { "Name": "Grace", "Class": "grace", "Designation": "Development Manager", "About": "Grace maintains training plans to achive workforce skill." },
        { "Name": "Jacob", "Class": "jacob", "Designation": "Recruitment Manager", "About": "Jacob manages recruitment and prepares key staffing metrics." }];


{% endhighlight %}



{% highlight css %}

     .sample-control.template .e-m-lv-item {
    height: 85px;
    width: 100%;
    padding: 4px 0px;
}

    .sample-control.template .e-m-lv-item .cont-bg {
        padding-top: 10px;
        padding-left: 5px;
    }

.sample-control.template .designationstyle {
    float: right;
    font-size: 12px;
    position: relative;
    right: 25px;
    padding-top: 5px;
}

.sample-control.template .aboutstyle {
    display: block;
    font-size: 14px;
    line-height: 20px;
    overflow: hidden;
    padding-left: 10px;
    padding-right: 5px;
    text-align: justify;
}

.sample-control.template .templatetext {
    font-weight: bolder;
    position: relative;
    font-size: 17px;
    margin-left: 10px;
}

.sample-control.template .listrightdiv {
    position: relative;
}

.sample-control.template .e-m-lv-active .listrightdiv {
    color: white;
}

.sample-control.template .e-m-lv-item .brooke {
    background-image: url('sampleimages/Employees/1.png');
}

.sample-control.template .e-m-lv-item .claire {
    background-image: url('sampleimages/Employees/2.png');
}

.sample-control.template .e-m-lv-item .erik {
    background-image: url('sampleimages/Employees/3.png');
}

.sample-control.template .e-m-lv-item .grace {
    background-image: url('sampleimages/Employees/4.png');
}

.sample-control.template .e-m-lv-item .jacob {
    background-image: url('sampleimages/Employees/5.png');
}

.sample-control.template .profile {
    background-repeat: no-repeat;
    background-size: 49px 48px;
    border: 1px solid #e5e5e5;
    float: left;
    height: 52px;
    position: relative;
    width: 50px;
}


{% endhighlight %}

![](templating_images\templating_img1.png)

