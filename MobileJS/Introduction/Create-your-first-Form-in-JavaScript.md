---
layout: post
title: Create your first Form in JavaScript | Introduction | Mobilejs | Syncfusion
description: create your first form in javascript
platform: Mobilejs
control: Introduction
documentation: ug
---

# Create your first Form in JavaScript

The Essential JavaScript provides a way to create a Form with the following EJ mobile widgets.

1. Textbox 
2. Numeric Textbox
3. Radiobutton 
4. Checkbox 
5. Button

In the following guidelines, you are creating a Bill Payment App through that you can learn about the features in the above mentioned widgets.

![](getting-started_images/getting-started_img1.png)

Bill Payment App
{:.caption}

![](getting-started_images/getting-started_img2.png)

Bill Payment App
{:.caption}

### Create the necessary layout 

In the Bill Payment App, you can use the Textbox control to get the Name of the Person, Email, and Remarks, Numeric Textbox control for Amount field, Radio button for Payment options, Checkbox for the terms and conditions, and Button control to submit the Form. Also you can use the Dialog control for validation and Navigation header on top.

Create an HTML file and paste the following template to it to create a Form.

{% highlight html %}


    <div id="header" data-ej-title="Bill Payment" data-role="ejmnavigationbar"></div>
    <div id="ScrollPanel" data-role="ejmscrollpanel">
        <div id="form_sample" class="sample">
            <!--Add Form Element Here-->
            <form id="form1">
                <label>
                    Name of the Person:
                </label>
                <br /><br />
                <div>
                    <!--Textbox-->
                </div>
                <br />
                <label>
                    Amount:
                </label>
                <br /><br />
                <div>
                    <!--Numeric Textbox-->
                </div>
                <br />
                <div>
                    <label>
                        Payment Option:
                    </label>
                </div>
                <br />
                <div>
                    <table class="radio">
                        <tr>
                            <td>
                                <!--Radio Button for Credit-->
                            </td>
                            <td>
                                <!--Radio Button for Debit-->
                            </td>
                        </tr>
                    </table>
                </div>
                <br />
                <label>
                    Email:
                </label>
                <br /><br />
                <div>
                    <!--Add Email Textbox here-->
                </div>
                <br />
                <label>
                    Remarks (Optional):
                </label>
                <br /><br />
                <div>
                    <!--Add Remarks Textbox here-->
                </div>
                <br />
                <div>
                    <table class="check">
                        <tr>
                            <td>
                                <!--Add check box here-->
                            </td>
                        </tr>
                    </table>
                </div>
                <br />
                <div align="center" class="submitbutton">
                    <!--Add submit button here-->
                </div>
            </form>
        </div>
    </div>

    <!--Add dialog control here-->
    <div id="info_msg" data-role="ejmdialog" data-ej-title="Alert" data-ej-leftbuttoncaption="Ok" data-ej-buttontap="exit" data-ej-enablemodal="true">
        <div id="dlgcontent"></div>
    </div>



{% endhighlight %}



Add the following styles.

{% highlight html %}


    <style>
        .sample {
            padding: 16px;
        }

            .sample .submitbutton {
                text-align: center;
            }

            .sample .chksample {
                display: inline-block;
            }

            .sample label.error {
                color: #FF0000;
            }

        .check td, .radio td {
            min-width: 150px;
        }
    </style>



{% endhighlight %}

   

### Add Textbox Control

To render the Textbox control, you need to set “data-role” attribute to “ejmtextbox” to an “input” element.

{% highlight html %}


                    <!--Textbox-->
                    <input id="user_name" data-ej-type="text" data-role="ejmtextbox" required />
                    <label for="user_name" class="error" generated="true" />



{% endhighlight %}

Run this code and you can see the following output.

![](getting-started_images/getting-started_img3.png)

Form with Essential JS Mobile Textbox
{:.caption}

### Set Watermark text

The watermark text specifies a short hint that describes the expected value of the input field. This can be achieved by using the “data-ej-watermarktext” attribute.

{% highlight html %}


                    <input id="user_name" data-ej-type="text" data-role="ejmtextbox" data-ej-watermarktext="User name" required />



{% endhighlight %}

![](getting-started_images/getting-started_img4.png)

Form with Essential JS Mobile Textbox control with watermark text
{:.caption}

### Add Numeric Textbox Control

To render the Numeric Textbox control, you need to set “data-role” attribute to “ejmnumeric” to an “input” element and set its type attribute to number.

{% highlight html %}


                    <!--Numeric Textbox-->
                    <input id="amount" data-role="ejmnumeric" data-ej-type="number" required />
                    <label for="amount" class="error" generated="true" />



{% endhighlight %}

![](getting-started_images/getting-started_img5.png)

Form with Essential JS Mobile Numeric Textbox control
{:.caption}


A Radio Button control is required for the payment option (credit or debit). To render this control, set data-role attribute to ejmradiobutton to an input element and set its type attribute to radio. By using external label, you can set the text for Radio Button.

{% highlight html %}


                                <!--Radio Button for Credit-->
                                <input id="credit" name="payoption" data-role="ejmradiobutton" data-ej-checked="true" type="radio" />
                                <label for="credit" class="e-m-input-label">Credit Card</label>

                                <!--Radio Button for Debit-->
                                <input id="debit" name="payoption" data-role="ejmradiobutton" type="radio" />
                                <label for="debit" class="e-m-input-label">Debit Card</label>



{% endhighlight %}

![](getting-started_images/getting-started_img6.png)

Form with Essential JS Mobile Radio Button control
{:.caption}

### Add Textbox for E-mail

You can add Textbox for E-mail.

{% highlight html %}


                    <!--Add Email Textbox here-->
                    <input id="mail" name="mail" data-role="ejmtextbox" data-ej-watermarktext="user@mail.com" data-ej-type="email" required />
                    <label for="mail" class="error" generated="true" />



{% endhighlight %}

![](getting-started_images/getting-started_img7.png)

Form with Essential JS Mobile Textbox control
{:.caption}

You can add Textbox for Remarks.

{% highlight html %}


                    <!--Add Remarks Textbox here-->
                    <input name="remarks" data-role="ejmtextbox" data-ej-type="text" data-ej-watermarktext="Remarks" />



{% endhighlight %}

![](getting-started_images/getting-started_img8.png)

Form with Essential JS Mobile
{:.caption}

### Add Checkbox Control

You can use Checkbox Control for “agree the terms and conditions” option. To render this, set data-role attribute to ejmcheckbox to an input element and set its type attribute to checkbox. By using external labels, you can set the text for the Check box.

{% highlight html %}


                                <!--Add check box here-->
                                <input id="chkbox" data-role="ejmcheckbox" type="checkbox" />
                                <label for="chkbox" class="e-m-input-label">I accept the terms and conditions</label>




{% endhighlight %}

![](getting-started_images/getting-started_img9.png)

Form with Essential JS Mobile Checkbox control
{:.caption}

### Add Button Control

You require a Button Control to submit the Form. To render this control, set data-role attribute to ejmbutton to an “input” element. Add the data-ej-text attribute to specify the Button text. By using data-ej-touchend attribute, you can handle the form validation on button click.

{% highlight html %}


                    <!--Add submit button here-->
                    <input id="btn" name="submit" data-role="ejmbutton" data-ej-text="Pay Bill" type="button" data-ej-touchend="formsubmit" />



{% endhighlight %}

![](getting-started_images/getting-started_img10.png)

Form with Essential JS Mobile Button
{:.caption}

### Form Validation

The Bill payment is created with required controls and for validation, Essential JavaScript Mobile Dialog control is used to show the status of your payment. Add the below script to your page.

{% highlight html %}


    <script type="text/javascript">

        function formsubmit(event) {
            validation();
            $("#form1").submit();
        }

        function exit() {
            if ($("#chkbox").ejmCheckBox("isChecked")) {
                $(".sample input").val("");
                $("#chkbox").ejmCheckBox("model.checked", false);
                $("#btn").val("Pay Bill");
            }
            var dialogObject = $("#info_msg").data("ejmDialog"); // creating instance for dialog
            dialogObject.close(); // close dialog
        }

        function validation() {
            validator = $("#form1").validate({
                debug: true,
                messages: {
                    user_name: { required: "Please enter user name" },
                    amount: { required: "Please enter amount" },
                    mail: { required: "Please enter e-mail" }
                },
                submitHandler: function (form) {
                    var dialogObject = $("#info_msg").data("ejmDialog"); // creating instance for dialog
                    if (!$("#chkbox").ejmCheckBox("isChecked")) {
                        dialogObject.open(); // open dialog
                        $("#dlgcontent").text("Could you please agree our terms and conditions ?");
                    }
                    else {
                        dialogObject.open();
                        $("#dlgcontent").text("Your payment is received successfully");
                    }
                }
            });
        }

    </script>



{% endhighlight %}

![](getting-started_images/getting-started_img11.png)

Form submission without enter any values
{:.caption}

![](getting-started_images/getting-started_img12.png)

Submission with values without acceptance
{:.caption}

![](getting-started_images/getting-started_img13.png)

Final submission with proper values
{:.caption}

From the above steps, you have learnt how to create and customize Essential JS mobile Textbox, Numeric Textbox, Maskedit, Radiobutton, checkbox and Button widgets with use case samples. We have more customization properties other than the one used here. To know more about the properties in mentioned mobile widgets please refer the complete documentation page.