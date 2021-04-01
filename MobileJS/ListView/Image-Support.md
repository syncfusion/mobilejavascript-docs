---
layout: post
title: image-support
description: image support
platform: js
control: ListView
documentation: ug
---

## Image support

You can add images to your ListView items by specifying the image class name for individual items using ‘data-ej-fields-image’ attribute.

The following code example displays how to add images to the ListView.

{% highlight html %}

  <ul id="listview" data-role="ejmlistview" data-ej-datasource="window.listData" data-ej-fields-text="text" data-ej-fields-image="image" ></ul>
    <script>	
        window.listData = [{ text: "Australia", image: "Australia.png" },
                           { text: "Brazil", image: "Brazil.png" },
                           { text: "China", image: "china.png" },
                           { text: "India", image: "India.png" },
                           { text: "Spain", image: "Spain.png" }];
    </script>


{% endhighlight %}

![](image-support_images\image-support_img1.png)

