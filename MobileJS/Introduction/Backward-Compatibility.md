---
layout: post
title: Backward Compatibility | Introduction | Mobilejs | Syncfusion
description: backward compatibility
platform: Mobilejs
control: Introduction
documentation: ug
---

# Backward Compatibility


## Version 14.1.0.41 Changes

As a part of an effort to improve the user experience and provide consistent APIs across all the Syncfusion’s controls, significant changes are made to the API naming effective from Volume 1, 2016 release. The changes have been documented with mapping between the old and new API names to enable quick up gradation of any control. To migrate from Volume 1, 2016 or from earlier, refer to the following specified API changes.


## Common


### Features

* Provides en-US Locale text object, which gives user flexibility to convert it or create their own local language object with some simple modifications.

### Breaking Changes

* Check controls list to know about the list of API’s removed or modified in this release.


## ejmAccordion

### Breaking Changes

* Check the below table for ejmAccordion API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
collapsible</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
selectedItems</td><td>
selectedItems</td><td>
No Changes</td></tr>
<tr>
<td>
disabledItems</td><td>
disabledItems</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
expandAll</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
collapseAll</td><td>
Newly Added</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
heightAdjustMode</td><td>
heightAdjustMode</td><td>
No Changes</td></tr>
<tr>
<td>
showHeaderIcon</td><td>
showHeaderIcon</td><td>
No Changes</td></tr>
<tr>
<td>
enableCache</td><td>
enableCache</td><td>
No Changes</td></tr>
<tr>
<td>
enableMultipleOpen</td><td>
enableMultipleOpen</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
headerIcon: {normal,active}</td><td>
Newly Added</td></tr>
<tr>
<td>
spinnerText</td><td>
spinnerText</td><td>
No Changes</td></tr>
<tr>
<td>
windows: {renderDefault}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
items</td><td>
items</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
enableRippleEffect</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
enableAjax</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
prefetchAjaxContent</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
showAjaxPopup</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
itemTouchStart</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
itemTouchEnd</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
select</td><td>
Newly Added</td></tr>
<tr>
<td>
active</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
beforeActive</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
ajaxLoad</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
ajaxBeforeLoad</td><td>
ajaxBeforeLoad</td><td>
No Changes</td></tr>
<tr>
<td>
ajaxSuccess</td><td>
ajaxSuccess</td><td>
No Changes</td></tr>
<tr>
<td>
ajaxError</td><td>
ajaxError</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
expand</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
collapse</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
ajaxComplete</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
ajaxSettings: {type,cache,async,dataType,contentType,url,data}</td><td>
Newly Added</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enableItems</td><td>
enableItems</td><td>
No Changes</td></tr>
<tr>
<td>
disableItems</td><td>
disableItems</td><td>
No Changes</td></tr>
<tr>
<td>
show</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
hide</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
selectItems</td><td>
selectItems</td><td>
No Changes</td></tr>
<tr>
<td>
deselectItems</td><td>
deselectItems</td><td>
No Changes</td></tr>
<tr>
<td>
collapseAll</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
expandAll</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getItemsCount</td><td>
getItemsCount</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
addItem</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
removeItem</td><td>
Newly Added</td></tr>
</table>



## ejmAutoComplete

### Breaking Changes

* Check the below table for ejmAutoComplete API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
allowScrolling</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
windows: {renderDefault}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
filterType</td><td>
filterType</td><td>
No Changes</td></tr>
<tr>
<td>
caseSensitiveSearch</td><td>
caseSensitiveSearch</td><td>
No Changes</td></tr>
<tr>
<td>
enableAutoFill</td><td>
enableAutoFill</td><td>
No Changes</td></tr>
<tr>
<td>
delimiterChar</td><td>
delimiterChar</td><td>
No Changes</td></tr>
<tr>
<td>
enableMultiSelect</td><td>
enableMultiSelect</td><td>
No Changes</td></tr>
<tr>
<td>
enableCheckbox</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
dataSource</td><td>
dataSource</td><td>
No Changes</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
itemsCount</td><td>
itemsCount</td><td>
No Changes</td></tr>
<tr>
<td>
fields: {text,key}</td><td>
fields: {text,key,image}</td><td>
Renamed</td></tr>
<tr>
<td>
selectedKeys</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
imageField</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
mapper</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
watermarkText</td><td>
watermarkText</td><td>
No Changes</td></tr>
<tr>
<td>
imageClass</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
allowSorting</td><td>
allowSorting</td><td>
No Changes</td></tr>
<tr>
<td>
sortOrder</td><td>
sortOrder</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
emptyResultText</td><td>
emptyResultText</td><td>
No Changes</td></tr>
<tr>
<td>
showEmptyResultText</td><td>
showEmptyResultText</td><td>
No Changes</td></tr>
<tr>
<td>
minCharacter</td><td>
minCharacter</td><td>
No Changes</td></tr>
<tr>
<td>
enableDistinct</td><td>
enableDistinct</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
popupWidth</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
popupHeight</td><td>
Newly Added</td></tr>
<tr>
<td>
Mode</td><td>
Mode</td><td>
No Changes</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
keyPress</td><td>
keyPress</td><td>
No Changes</td></tr>
<tr>
<td>
select</td><td>
select</td><td>
No Changes</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
<tr>
<td>
focusOut</td><td>
focusOut</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
<tr>
<td>
getValue</td><td>
getValue</td><td>
No Changes</td></tr>
<tr>
<td>
getSelectedItems</td><td>
getSelectedItems</td><td>
No Changes</td></tr>
<tr>
<td>
clearText</td><td>
clearText</td><td>
No Changes</td></tr>
</table>



## ejmButton

### Breaking Changes

* Check the below table for ejmButton API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
text</td><td>
text</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
href</td><td>
href</td><td>
No Changes</td></tr>
<tr>
<td>
imageClass</td><td>
imageClass</td><td>
No Changes</td></tr>
<tr>
<td>
imagePosition</td><td>
imagePosition</td><td>
No Changes</td></tr>
<tr>
<td>
contentType</td><td>
contentType</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
ios7: {”style”: “normal”}, android: {”style”: “normal”}, windows: {”style”: “normal”}, flat: {”style”: “normal”}</td><td>
style:{header,back,large,normal}</td><td>
Renamed</td></tr>
<tr>
<td>
ios7: {”color”: “ “,}</td><td>
color:{border,fill,text}</td><td>
Renamed</td></tr>
<tr>
<td>
windows:{”renderDefault”: false}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
inline</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
inline</td><td>
enableRippleEffect</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
showBorder</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
enableRippleEffect:,ej.isAndroid() ? true : false,</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
</table>



## ejmCheckBox

### Breaking Changes

* Check the below table for ejmCheckBox API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
checked</td><td>
checked</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
text</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
enableRippleEffect:ej.isAndroid? true : false</td><td>
Newly Added</td></tr>
<tr>
<td>
preventDefault</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableTriState</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
checkState</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows: {”renderDefault”: false}</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
beforeChange</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
change</td><td>
Newly Added</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
isChecked</td><td>
isChecked</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
enable</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
disable</td><td>
Newly Added</td></tr>
</table>



## ejmDatePicker

### Breaking Changes

* Check the below table for ejmDatePicker API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
dateFormat</td><td>
dateFormat</td><td>
No Changes</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
minDate</td><td>
minDate</td><td>
No Changes</td></tr>
<tr>
<td>
maxDate</td><td>
maxDate</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
culture</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
ios7: {renderDefaul}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows: {renderDefault}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
focusOut</td><td>
focusOut</td><td>
No Changes</td></tr>
<tr>
<td>
Load</td><td>
Load</td><td>
No Changes</td></tr>
<tr>
<td>
focusIn</td><td>
focusIn</td><td>
No Changes</td></tr>
<tr>
<td>
Open</td><td>
Open</td><td>
No Changes</td></tr>
<tr>
<td>
Change</td><td>
Change</td><td>
No Changes</td></tr>
<tr>
<td>
close</td><td>
close</td><td>
No Changes</td></tr>
<tr>
<td>
select</td><td>
select</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
show</td><td>
show</td><td>
No Changes</td></tr>
<tr>
<td>
hide</td><td>
hide</td><td>
No Changes</td></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
<tr>
<td>
getValue</td><td>
getValue</td><td>
No Changes</td></tr>
<tr>
<td>
setCurrentDate</td><td>
setCurrentDate</td><td>
No Changes</td></tr>
</table>



## ejmDialog

### Breaking Changes

* Check the below table for ejmDialog API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
templateId</td><td>
templateId</td><td>
No Change</td></tr>
<tr>
<td>
targetHeight</td><td>
height</td><td>
Renamed</td></tr>
<tr>
<td>
-</td><td>
width</td><td>
Newly Added</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Change</td></tr>
<tr>
<td>
enableAnimation</td><td>
enableAnimation</td><td>
No Change</td></tr>
<tr>
<td>
open</td><td>
open</td><td>
No Change</td></tr>
<tr>
<td>
close</td><td>
close</td><td>
No Change</td></tr>
<tr>
<td>
beforeClose</td><td>
beforeClose</td><td>
No Change</td></tr>
<tr>
<td>
buttonTap</td><td>
buttonTap</td><td>
No Change</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
Windows{“renderDefault”:[]}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
mode</td><td>
mode</td><td>
No Change</td></tr>
<tr>
<td>
enableAutoOpen</td><td>
enableAutoOpen</td><td>
No Change</td></tr>
<tr>
<td>
title</td><td>
title</td><td>
No Change</td></tr>
<tr>
<td>
-</td><td>
closeOndocumentTap</td><td>
Newly Added</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Change</td></tr>
<tr>
<td>
enableModal</td><td>
enableModal</td><td>
No Change</td></tr>
<tr>
<td>
showButtons</td><td>
showButtons</td><td>
No Change</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Change</td></tr>
<tr>
<td>
leftButtonCaption</td><td>
leftButtonCaption</td><td>
No Change</td></tr>
<tr>
<td>
rightButtonCaption</td><td>
rightButtonCaption</td><td>
No Change</td></tr>
<tr>
<td>
allowScrolling</td><td>
allowScrolling</td><td>
No Change</td></tr>
<tr>
<td>
enableNativeScrolling</td><td>
enableNativeScrolling</td><td>
No Change</td></tr>
<tr>
<td>
checkDOMChanges</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
showHeader</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
open</td><td>
open</td><td>
No Changes</td></tr>
<tr>
<td>
close</td><td>
close</td><td>
No Changes</td></tr>
<tr>
<td>
beforeclose</td><td>
beforeClose</td><td>
No Changes</td></tr>
<tr>
<td>
buttonTap</td><td>
buttonTap</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
open</td><td>
open</td><td>
No Change</td></tr>
<tr>
<td>
close</td><td>
close</td><td>
No Change</td></tr>
<tr>
<td>
isOpened</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
disableButton</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
enableButton</td><td>
Newly Added</td></tr>
</table>



## ejmDropdownList

### Breaking Changes

* Check the below table for ejmDropdownList API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
<tr>
<td>
targetID</td><td>
targetID</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
templateId</td><td>
Newly Added</td></tr>
<tr>
<td>
selectedItemIndex</td><td>
selectedItemIndex</td><td>
No Changes</td></tr>
<tr>
<td>
dataSource</td><td>
dataSource</td><td>
No Changes</td></tr>
<tr>
<td>
fields: {text,groupBy,imageClass,imageUrl,checkBy,enableTemplate,templateID,value}</td><td>
fields: {text,value,groupBy,image,checkBy}</td><td>
Changed</td></tr>
<tr>
<td>
query</td><td>
query</td><td>
No Changes</td></tr>
<tr>
<td>
allowVirtualScrolling</td><td>
allowVirtualScrolling</td><td>
No Changes</td></tr>
<tr>
<td>
virtualScrollMode</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
itemRequestCount</td><td>
ItemsCount</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
enableMultiSelect</td><td>
enableMultiSelect</td><td>
No Changes</td></tr>
<tr>
<td>
delimiterChar</td><td>
delimiterChar</td><td>
No Changes</td></tr>
<tr>
<td>
enableGrouping</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
mode</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableTemplate</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows: {type}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
android: {popUpHeight}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
items</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
waterMarkText</td><td>
waterMarkText</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
popupHeight</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
popupWidth</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
 -</td><td>
actionSuccess</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
actioinFailure</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
actioinComplete</td><td>
Newly Added</td></tr>
<tr>
<td>
focusIn</td><td>
focusIn</td><td>
No Changes</td></tr>
<tr>
<td>
focusOut</td><td>
focusOut</td><td>
No Changes</td></tr>
<tr>
<td>
select</td><td>
seelect</td><td>
No Changes</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
<tr>
<td>
checkChange</td><td>
-</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
showPopup</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
hidePopup</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
getValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
selectItemByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
selectItemByIndices</td><td>
selectItemByIndices</td><td>
No Changes</td></tr>
<tr>
<td>
unselectItemByIndex</td><td>
unselectItemByIndex</td><td>
No Changes</td></tr>
<tr>
<td>
unselectItemByIndices</td><td>
unselectItemByIndices</td><td>
No Changes</td></tr>
<tr>
<td>
show</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
hide</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getSelectedItemValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getSelectedItemsValue</td><td>
-</td><td>
Removed</td></tr>
</table>



## ejmGrid

Features

*  151276 - Prevented the filtering text from overriding while using Ionic framework

### Breaking Changes

* Theme property has been removed from the ejmGrid


## ejmGroupButton

### Breaking Changes

* Check the below table for ejmGroupButton API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Change</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Change</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Change</td></tr>
<tr>
<td>
selectedItemIndex</td><td>
selectedItemIndex</td><td>
No Change</td></tr>
<tr>
<td>
items</td><td>
items</td><td>
No Change</td></tr>
<tr>
<td>
windows:</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Change</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Change</td></tr>
</table>



## ejmListView

### Breaking Changes

* Check the below table for ejmListView API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
 -</td><td>
dataSource</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
templateId</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
enabled</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
enableChecklist</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
persistSelection</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
allowSelection</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
checkedIndices</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
query</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
deleteMode</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
selectedIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
enablePersistence</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
itemsCount</td><td>
Newly Added</td></tr>
<tr>
<td>
 -</td><td>
cssClass</td><td>
Newly Added</td></tr>
<tr>
<td>
pullToRefreshSettings{pullText,releaseText, refreshText,errorText,appendData,appendPosition}</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
theme</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
refreshThreshold</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
enablePullToRefresh</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
showScrollbars</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
showHeaderBackButton</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
autoAdjustScrollHeight</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
autoAdjustHeight</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
mode</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
headerBackButtonTap</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
adjustFixedPosition</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
enableNativeScrolling</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
hideHeaderForUnsupportedDevice</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
transition</td><td>
 -</td><td>
Removed</td></tr>
<tr>
<td>
fieldSettings,{navigateUrl,href,enableAjax,preventSelection, persistSelection,text,enableCheckMark,checked, primaryKey,parentPrimaryKey,imageClass,imageUrl, childHeaderTitle,childId,childHeaderBackButtonText,, renderTemplate,templateId,touchStart,touchEnd, attributes,groupID,id,value}</td><td>
fields: {text,value,image,groupBy,checkBy,enabled,href, allowSelection,badge: {value,maxValue}}</td><td>
Changed</td></tr>
<tr>
<td>
ios7{inline}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
Windows{preventSkew,renderDefault,enableHeaderCustomText}</td><td>
windows: {preventSkew}</td><td>
Changed</td></tr>
<tr>
<td>
allowScrolling</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
items</td><td>
items</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
allowSelection</td><td>
Newly Added</td></tr>
<tr>
<td>
checkDOMChanges</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
refreshBegin</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refreshSuccess</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refreshError</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refreshComplete</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
select</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
beforeDelete</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
afterDelete</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
actionFailure</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
actionComplete</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
actionSuccess</td><td>
Newly Added</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
getSelectedItemValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getSelectedItemsValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
setBadge</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
deleteItemByText</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
deleteItemByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
getIndexByText</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
getTextByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
getItemByText</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
getItemByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
uncheckAll</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
checkAll</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
uncheckItemsByIndices</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
uncheckItemsByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
checkItemsByIndices</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
checkItemsByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
deselectItem</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
selectItemByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
disableAll</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
enableAll</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
disableItemsByIndices</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
enableItemsByIndices</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
enableItemByIndex</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
disable</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
enable</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
append</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
refresh</td><td>
Newly Added</td></tr>
</table>



## ejmMaskedit

### Breaking Changes

* Check the below table for ejmMaskedit API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
borderStyle</td><td>
Newly Added</td></tr>
<tr>
<td>
watermarkText</td><td>
watermarkText</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
type</td><td>
Newly Added</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
maxLength</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
autoFocus</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
height</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
width</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
step</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
minValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
maxValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
format</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:,{renderDefault ,allowReset}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showBorder</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
mask</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
touchStart</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
touchEnd</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyUp</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyDown</td><td>
Newly Added</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getStrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getUnstrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getWatermarkText</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refresh</td><td>
-</td><td>
Removed</td></tr>
</table>



## ejmMenu

### Breaking Changes

* Check the below table for ejmMenu API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
width</td><td>
width</td><td>
No Changes</td></tr>
<tr>
<td>
height</td><td>
height</td><td>
No Changes</td></tr>
<tr>
<td>
allowScrolling</td><td>
allowScrolling</td><td>
No Changes</td></tr>
<tr>
<td>
targetId</td><td>
target</td><td>
Renamed</td></tr>
<tr>
<td>
target</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showOn</td><td>
showOn</td><td>
No Changes</td></tr>
<tr>
<td>
ios7: {”type”: “auto”,”showTitle”: true,”title”: “Title”, “showCancelButton”: true,”cancelButtonText”: “Cancel”, “cancelButtonColor”: “blue”,”cancelButtonTouchEnd”: null},</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
android: {”type”: “contextual”},</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows: {”type”: “contextual”,”renderDefault”: false},</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
renderTemplate</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showScrollbars</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
templateId</td><td>
templateId</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
dataSource</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
fields: {text: “”,href: null,color: “” }</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
query</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
text</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
color</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
cancelButton: {text: null,show: true,color: “”},</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
showTitle</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
title</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
showArrow</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
type :{actionSheet,popOver,popUp}</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
enableRippleEffect: ej.isAndroid() ? true : false</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
href</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
actionSuccess</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
actionFailure</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
actionComplete</td><td>
Newly Added</td></tr>
<tr>
<td>
load</td><td>
load</td><td>
No Changes</td></tr>
<tr>
<td>
loadComplete</td><td>
loadComplete</td><td>
No Changes</td></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
hide</td><td>
hide</td><td>
No Changes</td></tr>
<tr>
<td>
show</td><td>
show</td><td>
No Changes</td></tr>
<tr>
<td>
items</td><td>
items</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
show</td><td>
show</td><td>
No Changes</td></tr>
<tr>
<td>
hide</td><td>
hide</td><td>
No Changes</td></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
<tr>
<td>
enableItem</td><td>
enableItem</td><td>
No Changes</td></tr>
<tr>
<td>
disableItem</td><td>
disableItem</td><td>
No Changes</td></tr>
<tr>
<td>
enableOverFlowItem</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disableOverFlowItem</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableOverFlow</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disableOverFlow</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
addItem</td><td>
addItem</td><td>
No Changes</td></tr>
<tr>
<td>
removeItem</td><td>
removeItem</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
enableCancelButton</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
disableCancelButton</td><td>
Newly Added</td></tr>
</table>



## ejmNavigationBar

### Breaking Changes

* Check the below table for ejmNavigationBar API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
hideForUnSupportedDevice</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
leftButtonNavigationUrl</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
leftButtonImageClass</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
leftButtonImageUrl</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightButtonNavigationUrl</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightButtonImageClass</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightButtonImageUrl</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showTitle</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
position</td><td>
isRelative</td><td>
Renamed</td></tr>
<tr>
<td>
title</td><td>
title</td><td>
No Changes</td></tr>
<tr>
<td>
leftButtonCaption</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightButtonCaption</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showLeftButton</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showRightButton</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
android: {”backButtonImageClass”:null,”leftButtonStyle”: “auto”, “rightButtonStyle”: “auto”,”showLeftButton”: false, “showRightButton”: false,”showBackNavigator”: false, “position”:”auto”,”showTitleIcon”: false, “enableSplitView”: false,”titleIconUrl”: “”, “showEllipsis”: false,”title”: “Title”},</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
templateId</td><td>
templateId</td><td>
No Changes</td></tr>
<tr>
<td>
windows: {”renderDefault”: false,”enableCustomText”: false, “leftButtonStyle”: “auto”,”rightButtonStyle”: “auto”, “showLeftButton”: false,”showRightButton”: false},</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
flat: {”leftButtonStyle”: “auto”,”rightButtonStyle”: “auto”, “showLeftButton”: false,”showRightButton”: false}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
ios7: {”leftButtonStyle”: “auto”,”rightButtonStyle”: “auto”, “showLeftButton”: false,”showRightButton”: false}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
leftButtonStyle</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightButtonStyle</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
layout</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
hide</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
android: {”showBackNavigator”: false, “showTitleIcon”: false,”enableSplitView”: false, “titleIconUrl”: “”,”showEllipsis”: false,”title”: “Title”}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
position: {Top,Bottom}</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
iconAlignment: {Center,Left,Right}</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
titleAlignment: {Center,Left,Right}</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
badge.maxValue</td><td>
Newly Added</td></tr>
<tr>
<td>
items</td><td>
items</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
enableRippleEffect</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
mode</td><td>
Newly Added</td></tr>
<tr>
<td>
enabled</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
leftButtonTap</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightButtonTap</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
ellipsisTouchStart</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
ellipsisTouchEnd</td><td>
Newly Added</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
getTitle</td><td>
getTitle</td><td>
No Changes</td></tr>
<tr>
<td>
removeItem</td><td>
removeItem</td><td>
No Changes</td></tr>
<tr>
<td>
addItem</td><td>
addItem</td><td>
No Changes</td></tr>
<tr>
<td>
showEllipsis</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
hideEllipsis</td><td>
-</td><td>
No Changes</td></tr>
<tr>
<td>
disableItem</td><td>
disableItem</td><td>
No Changes</td></tr>
<tr>
<td>
enableItem</td><td>
enableItem</td><td>
No Changes</td></tr>
<tr>
<td>
hideItem</td><td>
hideItem</td><td>
No Changes</td></tr>
<tr>
<td>
showItem</td><td>
showItem</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
hide</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
show</td><td>
 </td></tr>
<tr>
<td>
hideMenu</td><td>
-</td><td>
No Changes</td></tr>
<tr>
<td>
showMenu</td><td>
-</td><td>
No Changes</td></tr>
</table>



## ejmNumeric

### Breaking Changes

* Check the below table for ejmNumeric API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
borderStyle</td><td>
Newly Added</td></tr>
<tr>
<td>
watermarkText</td><td>
watermarkText</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
type</td><td>
Newly Added</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
maxLength</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
autoFocus</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
height</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
width</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
step</td><td>
Newly Added</td></tr>
<tr>
<td>
minValue</td><td>
minValue</td><td>
No Changes</td></tr>
<tr>
<td>
maxValue</td><td>
maxValue</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
format</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:,{renderDefault ,allowReset}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showBorder</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showSpinButton</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
decimalPlaces</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableStrictMode</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
incrementStep</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
name</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
touchStart</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
touchEnd</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyUp</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyDown</td><td>
Newly Added</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
setValue</td><td>
-</td><td>
Removed</td></tr>
</table>



## ejmPassword

### Breaking Changes

* Check the below table for ejmPassword API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
borderStyle</td><td>
Newly Added</td></tr>
<tr>
<td>
watermarkText</td><td>
watermarkText</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
type</td><td>
Newly Added</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
maxLength</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
autoFocus</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
height</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
width</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
step</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
minValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
maxValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
format</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:,{renderDefault ,allowReset}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showBorder</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
mask</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
touchStart</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
touchEnd</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyUp</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyDown</td><td>
Newly Added</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getStrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getUnstrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getWatermarkText</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refresh</td><td>
-</td><td>
Removed</td></tr>
</table>



## ejmProgressBar

### Breaking Changes

* Check the below table for ejmProgressBar API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
percentage</td><td>
percentage</td><td>
No Changes</td></tr>
<tr>
<td>
incrementStep</td><td>
incrementStep</td><td>
No Changes</td></tr>
<tr>
<td>
minValue</td><td>
minValue</td><td>
No Changes</td></tr>
<tr>
<td>
maxValue</td><td>
maxValue</td><td>
No Changes</td></tr>
<tr>
<td>
width</td><td>
width</td><td>
No Changes</td></tr>
<tr>
<td>
height</td><td>
height</td><td>
No Changes</td></tr>
<tr>
<td>
orientation</td><td>
orientation</td><td>
No Changes</td></tr>
<tr>
<td>
text</td><td>
text</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
enableCustomText</td><td>
enableCustomText</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
theme</td><td>
No Changes</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
create</td><td>
create</td><td>
No Changes</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
<tr>
<td>
complete</td><td>
complete</td><td>
No Changes</td></tr>
<tr>
<td>
start</td><td>
start</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
getPercentage</td><td>
getPercentage</td><td>
No Changes</td></tr>
<tr>
<td>
setCustomText</td><td>
setCustomText</td><td>
No Changes</td></tr>
<tr>
<td>
changeEventHandler</td><td>
changeEventHandler</td><td>
No Changes</td></tr>
<tr>
<td>
getValue</td><td>
getValue</td><td>
No Changes</td></tr>
</table>



## ejmRadialMenu

### Breaking Changes

* Check the below table for ejmRadialMenu API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
imageClass</td><td>
imageClass</td><td>
No Changes</td></tr>
<tr>
<td>
backImageClass</td><td>
backImageClass</td><td>
No Changes</td></tr>
<tr>
<td>
position</td><td>
position</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows: {”renderDefault”: false}</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touch</td><td>
touch</td><td>
No Changes</td></tr>
<tr>
<td>
select</td><td>
select</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
documentClick</td><td>
documentClick</td><td>
No Changes</td></tr>
<tr>
<td>
menuHide</td><td>
menuHide</td><td>
No Changes</td></tr>
<tr>
<td>
showRadialMenu</td><td>
showRadialMenu</td><td>
No Changes</td></tr>
<tr>
<td>
resize</td><td>
resize</td><td>
No Changes</td></tr>
</table>



## ejmRadialSlider

### Breaking Changes

* Check the below table for ejmRadialSlider API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
theme</td><td>
No Changes</td></tr>
<tr>
<td>
position</td><td>
position</td><td>
No Changes</td></tr>
<tr>
<td>
strokeWidth</td><td>
strokeWidth</td><td>
No Changes</td></tr>
</table>



## ejmRadioButton

### Breaking Changes

* Check the below table for ejmRadioButton API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
checked</td><td>
checked</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
text</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
enableRippleEffect:ej.isAndroid? true : false</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
beforeChange</td><td>
Newly Added</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
isChecked</td><td>
Newly Added</td></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
</table>



## ejmRating

### Breaking Changes

* Check the below table for ejmRating API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
maxValue</td><td>
maxValue</td><td>
No Changes</td></tr>
<tr>
<td>
minValue</td><td>
minValue</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
incrementStep</td><td>
incrementStep</td><td>
No Changes</td></tr>
<tr>
<td>
precision</td><td>
precision</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
theme</td><td>
No Changes</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
shape</td><td>
shape</td><td>
No Changes</td></tr>
<tr>
<td>
shapeWidth</td><td>
shapeWidth</td><td>
No Changes</td></tr>
<tr>
<td>
shapeHeight</td><td>
shapeHeight</td><td>
No Changes</td></tr>
<tr>
<td>
spaceBetweenShapes</td><td>
spaceBetweenShapes</td><td>
No Changes</td></tr>
<tr>
<td>
orientation</td><td>
orientation</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
backgroundColor</td><td>
backgroundColor</td><td>
No Changes</td></tr>
<tr>
<td>
selectionColor</td><td>
selectionColor</td><td>
No Changes</td></tr>
<tr>
<td>
hoverColor</td><td>
hoverColor</td><td>
No Changes</td></tr>
<tr>
<td>
borderColor</td><td>
borderColor</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
tap</td><td>
tap</td><td>
No Changes</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
<tr>
<td>
touchMove</td><td>
touchMove</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
<tr>
<td>
show</td><td>
show</td><td>
No Changes</td></tr>
<tr>
<td>
hide</td><td>
hide</td><td>
No Changes</td></tr>
<tr>
<td>
getValue</td><td>
getValue</td><td>
No Changes</td></tr>
<tr>
<td>
reset</td><td>
reset</td><td>
No Changes</td></tr>
<tr>
<td>
setValue</td><td>
setValue</td><td>
No Changes</td></tr>
</table>



## ejmRotator

### Breaking Changes

* Check the below table for ejmRotator API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Changes</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Change</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showHeader</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
targetHeight</td><td>
targetHeight</td><td>
No Change</td></tr>
<tr>
<td>
targetWidth</td><td>
targetWidth</td><td>
No Change</td></tr>
<tr>
<td>
adjustFixedPosition</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showTitle</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showPager</td><td>
showPager</td><td>
No Change</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Change</td></tr>
<tr>
<td>
pagerPosition: {”horizontal”: “bottom”,”vertical”: “right”}</td><td>
pagerPosition=”bottom”</td><td>
No Change</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Change</td></tr>
<tr>
<td>
targetId</td><td>
targetId</td><td>
No Change</td></tr>
<tr>
<td>
swipeLeft</td><td>
swipeLeft</td><td>
No Change</td></tr>
<tr>
<td>
swipeRight</td><td>
swipeRight</td><td>
No Change</td></tr>
<tr>
<td>
swipeUp</td><td>
swipeUp</td><td>
No Change</td></tr>
<tr>
<td>
swipeDown</td><td>
swipeDown</td><td>
No Change</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Change</td></tr>
<tr>
<td>
pagerSelect</td><td>
pagerSelect</td><td>
No Change</td></tr>
<tr>
<td>
dataBinding</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
orientation</td><td>
orientation</td><td>
No Change</td></tr>
<tr>
<td>
windows: {”renderDefault”: false}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
dataSource</td><td>
dataSource</td><td>
No Change</td></tr>
<tr>
<td>
items</td><td>
items</td><td>
No Change</td></tr>
<tr>
<td>
currentItemIndex</td><td>
currentItemIndex</td><td>
No Change</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
swipeLeft</td><td>
swipeLeft</td><td>
No Changes</td></tr>
<tr>
<td>
swipeRight</td><td>
swipeRight</td><td>
No Changes</td></tr>
<tr>
<td>
swipeUp</td><td>
swipeUp</td><td>
No Changes</td></tr>
<tr>
<td>
swipeDown</td><td>
swipeDown</td><td>
No Changes</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
<tr>
<td>
pagerSelect</td><td>
pagerSelect</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderDatasource</td><td>
renderDatasource</td><td>
No Changes</td></tr>
</table>



## ejmScrollPanel

### Breaking Changes

* Check the below table for ejmScrollPanel API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Change</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableResize</td><td>
enableResize</td><td>
No Change</td></tr>
<tr>
<td>
targetHeight</td><td>
targetHeight</td><td>
No Change</td></tr>
<tr>
<td>
targetWidth</td><td>
targetWidth</td><td>
No Change</td></tr>
<tr>
<td>
scrollHeight</td><td>
scrollHeight</td><td>
No Change</td></tr>
<tr>
<td>
scrollWidth</td><td>
scrollWidth</td><td>
No Change</td></tr>
<tr>
<td>
enableFade</td><td>
enableFade</td><td>
No Change</td></tr>
<tr>
<td>
-</td><td>
allowPullToRefresh</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
cssClass</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
pullToRefreshSettings: {thresholdDistance: 75,textOnPull: “Pull to Refresh…”, textOnRelease: “Release to Refresh…“,textOnRefresh: “Refreshing…”}</td><td>
Newly Added</td></tr>
<tr>
<td>
autoAdjustHeight</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
isRelative</td><td>
isRelative</td><td>
No Change</td></tr>
<tr>
<td>
wheelSpeed</td><td>
wheelSpeed</td><td>
No Change</td></tr>
<tr>
<td>
enableInteraction</td><td>
enableInteraction</td><td>
No Change</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Change</td></tr>
<tr>
<td>
checkDOMChanges</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableHrScroll</td><td>
enableHrScroll</td><td>
No Change</td></tr>
<tr>
<td>
enableVrScroll</td><td>
enableVrScroll</td><td>
No Change</td></tr>
<tr>
<td>
eventPassthrough</td><td>
eventPassthrough</td><td>
No Change</td></tr>
<tr>
<td>
translateZ</td><td>
translateZ</td><td>
No Change</td></tr>
<tr>
<td>
zoomMin</td><td>
zoomMin</td><td>
No Change</td></tr>
<tr>
<td>
zoomMax</td><td>
zoomMax</td><td>
No Change</td></tr>
<tr>
<td>
adjustFixedPosition</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
mode</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
startZoom</td><td>
startZoom</td><td>
No Change</td></tr>
<tr>
<td>
startX</td><td>
startX</td><td>
No Change</td></tr>
<tr>
<td>
startY</td><td>
startY</td><td>
No Change</td></tr>
<tr>
<td>
enableDisplacement</td><td>
enableDisplacement</td><td>
No Change</td></tr>
<tr>
<td>
displacementValue</td><td>
displacementValue</td><td>
No Change</td></tr>
<tr>
<td>
displacementTime</td><td>
displacementTime</td><td>
No Change</td></tr>
<tr>
<td>
deceleration</td><td>
deceleration</td><td>
No Change</td></tr>
<tr>
<td>
disablePointer</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disableMouse</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disableTouch</td><td>
disableTouch</td><td>
No Change</td></tr>
<tr>
<td>
directionLockThreshold</td><td>
directionLockThreshold</td><td>
No Change</td></tr>
<tr>
<td>
momentum</td><td>
momentum</td><td>
No Change</td></tr>
<tr>
<td>
enableBounce</td><td>
enableBounce</td><td>
No Change</td></tr>
<tr>
<td>
bounceTime</td><td>
bounceTime</td><td>
No Change</td></tr>
<tr>
<td>
bounceEasing</td><td>
bounceEasing</td><td>
No Change</td></tr>
<tr>
<td>
preventDefault</td><td>
preventDefault</td><td>
No Change</td></tr>
<tr>
<td>
preventDefaultException</td><td>
preventDefaultException</td><td>
No Change</td></tr>
<tr>
<td>
enableTransition</td><td>
enableTransition</td><td>
No Change</td></tr>
<tr>
<td>
enableTransform</td><td>
enableTransform</td><td>
No Change</td></tr>
<tr>
<td>
showScrollbars</td><td>
showScrollbars</td><td>
No Change</td></tr>
<tr>
<td>
enableMouseWheel</td><td>
enableMouseWheel</td><td>
No Change</td></tr>
<tr>
<td>
enableKeys</td><td>
enableKeys</td><td>
No Change</td></tr>
<tr>
<td>
enableZoom</td><td>
enableZoom</td><td>
No Change</td></tr>
<tr>
<td>
enableNativeScrolling</td><td>
enableNativeScrolling</td><td>
No Change</td></tr>
<tr>
<td>
invertWheel</td><td>
invertWheel</td><td>
No Change</td></tr>
<tr>
<td>
enablePersistence</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableShrink</td><td>
enableShrink</td><td>
No Changes</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
scrollStart</td><td>
scrollStart</td><td>
No Changes</td></tr>
<tr>
<td>
scroll</td><td>
scroll</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
scrollStop</td><td>
Newly Added</td></tr>
<tr>
<td>
scrollEnd</td><td>
scrollEnd</td><td>
No Changes</td></tr>
<tr>
<td>
zoomStart</td><td>
zoomStart</td><td>
No Changes</td></tr>
<tr>
<td>
zoomEnd</td><td>
zoomEnd</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
pull</td><td>
Newly Added</td></tr>
<tr>
<td>
target</td><td>
target</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
zoom</td><td>
zoom</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
refresh</td><td>
refresh</td><td>
No Changes</td></tr>
<tr>
<td>
scrollBy</td><td>
scrollBy</td><td>
No Changes</td></tr>
<tr>
<td>
scrollTo</td><td>
scrollTo</td><td>
No Changes</td></tr>
<tr>
<td>
getComputedPosition</td><td>
getComputedPosition</td><td>
No Changes</td></tr>
<tr>
<td>
stop</td><td>
stop</td><td>
No Changes</td></tr>
<tr>
<td>
getScrollPosition</td><td>
getScrollPosition</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
closeRefresher</td><td>
Newly Added</td></tr>
</table>



## ejmSlider

### Breaking Changes

* Check the below table for ejmSlider API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
theme</td><td>
theme</td><td>
No Changes</td></tr>
<tr>
<td>
orientation</td><td>
orientation</td><td>
No Changes</td></tr>
<tr>
<td>
maxValue</td><td>
maxValue</td><td>
No Changes</td></tr>
<tr>
<td>
minValue</td><td>
minValue</td><td>
No Changes</td></tr>
<tr>
<td>
enableRange</td><td>
enableRange</td><td>
No Changes</td></tr>
<tr>
<td>
values</td><td>
values</td><td>
No Changes</td></tr>
<tr>
<td>
enableAnimation</td><td>
enableAnimation</td><td>
No Changes</td></tr>
<tr>
<td>
animationSpeed</td><td>
animationSpeed</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
<tr>
<td>
incrementStep</td><td>
incrementStep</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
windows: {”renderDefault”: false},</td><td>
windows: {”renderDefault”: false},</td><td>
No Changes</td></tr>
<tr>
<td>
ios7: {”thumbStyle”: “normal”},</td><td>
ios7: {”thumbStyle”: “normal”},</td><td>
No Changes</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
<tr>
<td>
slide</td><td>
slide</td><td>
No Changes</td></tr>
<tr>
<td>
load</td><td>
load</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
getValue</td><td>
getValue</td><td>
No Changes</td></tr>
<tr>
<td>
dispose</td><td>
dispose</td><td>
No Changes</td></tr>
</table>



## ejmSplitPane

### Breaking Changes

* Check the below table for ejmSplitPane API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
allowLeftPaneScrolling</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
allowRightPaneScrolling</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
leftPaneScrollSettings</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightPaneScrollSettings</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enablePersistence</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
android:</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
ios7:</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
flat:</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
leftHeaderSettings</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
rightHeaderSettings</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
overlayLeftPane</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
overlayDirection</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
leftPane:</td><td>
Newly Added</td></tr>
<tr>
<td>
enableSwipe</td><td>
enableSwipe</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
height</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
width</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
isRelative</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
edgeThreshold</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
stopEventPropagation</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
contentPane:</td><td>
Newly Added</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
afterLoadSuccess</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
beforeTransfer</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
swipe</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
open</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
close</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
beforeClose</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
beforeOpen</td><td>
Newly Added</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
loadContent</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
transferPage</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refreshRightScroller</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refreshLeftScroller</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
openLeftPane</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
closeLeftPane</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
closePane</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
openRightPane</td><td>
Newly Added</td></tr>
</table>



## ejmTab

### Breaking Changes

* Check the below table for ejmTab API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
enableAjax</td><td>
enableAjax</td><td>
No Changes</td></tr>
<tr>
<td>
enableCache</td><td>
enableCache</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
showAjaxPopup</td><td>
showAjaxPopup</td><td>
No Changes</td></tr>
<tr>
<td>
selectedItemIndex</td><td>
selectedItemIndex</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
prefetchAjaxContent</td><td>
prefetchAjaxContent</td><td>
No Changes</td></tr>
<tr>
<td>
ajaxSettings</td><td>
ajaxSettings</td><td>
No Changes</td></tr>
<tr>
<td>
items</td><td>
items</td><td>
No Changes</td></tr>
<tr>
<td>
badge.maxValue</td><td>
badge.maxValue</td><td>
No Changes</td></tr>
<tr>
<td>
ios7</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
android</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
widows</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
flat</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
badge.enabled</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
badge.value</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
badge.minValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
-</td><td>
position</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
itemStyle,enum:{BothBlock:”bothblock”,Image:”image”,Text:”text”, BothInline:”bothinline”}</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
allowSwiping</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
position</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
contentId</td><td>
Newly Added</td></tr>
<tr>
<td>
showScrollbars</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enableNativeScrolling</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
allowScrolling</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
load</td><td>
load</td><td>
No Changes</td></tr>
<tr>
<td>
loadComplete</td><td>
loadComplete</td><td>
No Changes</td></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
<tr>
<td>
ajaxBeforeLoad</td><td>
ajaxBeforeLoad</td><td>
No Changes</td></tr>
<tr>
<td>
ajaxError</td><td>
ajaxError</td><td>
No Changes</td></tr>
<tr>
<td>
ajaxComplete</td><td>
ajaxComplete</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
select</td><td>
Newly Added</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
showBadge</td><td>
showBadge</td><td>
No Changes</td></tr>
<tr>
<td>
hideBadge</td><td>
hideBadge</td><td>
No Changes</td></tr>
<tr>
<td>
updateBadgeValue</td><td>
updateBadgeValue</td><td>
Changed</td></tr>
<tr>
<td>
selectItem</td><td>
setActiveItem</td><td>
Changed</td></tr>
<tr>
<td>
enableItem</td><td>
enableItem</td><td>
No Changes</td></tr>
<tr>
<td>
disableItem</td><td>
disableItem</td><td>
No Changes</td></tr>
<tr>
<td>
enableContent</td><td>
enableContent</td><td>
No Changes</td></tr>
<tr>
<td>
disableContent</td><td>
disableContent</td><td>
No Changes</td></tr>
<tr>
<td>
addItem</td><td>
addItem</td><td>
No Changes</td></tr>
<tr>
<td>
removeItem</td><td>
removeItem</td><td>
No Changes</td></tr>
<tr>
<td>
getItemsCount</td><td>
getItemsCount</td><td>
No Changes</td></tr>
<tr>
<td>
getActiveItem</td><td>
getActiveItem</td><td>
No Changes</td></tr>
<tr>
<td>
getActiveItemText</td><td>
getActiveItemText</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
setContent</td><td>
Newly Added</td></tr>
<tr>
<td>
addOverflowItem</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
removeOverflowItem</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getOverflowItemCount</td><td>
-</td><td>
Removed</td></tr>
</table>



## ejmTextArea

### Breaking Changes

* Check the below table for ejmTextArea API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
borderStyle</td><td>
Newly Added</td></tr>
<tr>
<td>
watermarkText</td><td>
watermarkText</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
type</td><td>
Newly Added</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
maxLength</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
autoFocus</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
height</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
width</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
step</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
minValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
maxValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
format</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:,{renderDefault ,allowReset}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showBorder</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
mask</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
touchStart</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
touchEnd</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyUp</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyDown</td><td>
Newly Added</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getStrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getUnstrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getWatermarkText</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refresh</td><td>
-</td><td>
Removed</td></tr>
</table>



## ejmTextBox

### Breaking Changes

* Check the below table for ejmTextBox API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
borderStyle</td><td>
Newly Added</td></tr>
<tr>
<td>
watermarkText</td><td>
watermarkText</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
readOnly</td><td>
readOnly</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
type</td><td>
Newly Added</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
-</td><td>
maxLength</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
autoFocus</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
height</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
width</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
step</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
minValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
maxValue</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
format</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
locale</td><td>
Newly Added</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:,{renderDefault ,allowReset}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
showBorder</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
mask</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
-</td><td>
touchStart</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
touchEnd</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyUp</td><td>
Newly Added</td></tr>
<tr>
<td>
-</td><td>
keyDown</td><td>
Newly Added</td></tr>
<tr>
<td>
change</td><td>
-</td><td>
Removed</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
enable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
disable</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getStrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getUnstrippedValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getWatermarkText</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
getValue</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
refresh</td><td>
-</td><td>
Removed</td></tr>
</table>



## ejmTile

### Breaking Changes

* Check the below table for ejmTile API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
imagePath</td><td>
imagePath</td><td>
No Changes</td></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
ios7: {textPosition: “inner”},</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
android: {textPosition: “inner”}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
backgroundColor</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Changes</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Changes</td></tr>
</table>



## ejmTimePicker

### Breaking Changes

* Check the below table for ejmTimePicker API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Changes</td></tr>
<tr>
<td>
hourFormat</td><td>
hourFormat</td><td>
No Changes</td></tr>
<tr>
<td>
value</td><td>
value</td><td>
No Changes</td></tr>
<tr>
<td>
timeFormat</td><td>
timeFormat</td><td>
No Changes</td></tr>
<tr>
<td>
culture</td><td>
locale</td><td>
Renamed</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Changes</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Changes</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Changes</td></tr>
<tr>
<td>
ios7: {”renderDefault”: false}</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:{”renderDefault”: false}</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
select</td><td>
select</td><td>
No Changes</td></tr>
<tr>
<td>
load</td><td>
load</td><td>
No Changes</td></tr>
<tr>
<td>
focusIn</td><td>
focusIn</td><td>
No Changes</td></tr>
<tr>
<td>
focusOut</td><td>
focusOut</td><td>
No Changes</td></tr>
<tr>
<td>
open</td><td>
open</td><td>
No Changes</td></tr>
<tr>
<td>
close</td><td>
close</td><td>
No Changes</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Changes</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
show</td><td>
show</td><td>
No Changes</td></tr>
<tr>
<td>
hide</td><td>
hide</td><td>
No Changes</td></tr>
<tr>
<td>
getValue</td><td>
getValue</td><td>
No Changes</td></tr>
<tr>
<td>
setCurrentTime</td><td>
setCurrentTime</td><td>
No Changes</td></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Changes</td></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Changes</td></tr>
</table>



## ejmToggleButton

### Breaking Changes

* Check the below table for ejmToggleButton API Changes.

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
renderMode</td><td>
renderMode</td><td>
No Change</td></tr>
<tr>
<td>
theme</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
cssClass</td><td>
cssClass</td><td>
No Change</td></tr>
<tr>
<td>
enablePersistence</td><td>
enablePersistence</td><td>
No Change</td></tr>
<tr>
<td>
toggleState</td><td>
toggleState</td><td>
No Change</td></tr>
<tr>
<td>
enabled</td><td>
enabled</td><td>
No Change</td></tr>
<tr>
<td>
animate</td><td>
-</td><td>
Removed</td></tr>
<tr>
<td>
windows:</td><td>
-</td><td>
Removed</td></tr>
</table>
* Events

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
touchStart</td><td>
touchStart</td><td>
No Change</td></tr>
<tr>
<td>
touchEnd</td><td>
touchEnd</td><td>
No Change</td></tr>
<tr>
<td>
change</td><td>
change</td><td>
No Change</td></tr>
</table>
* Methods

<table>
<tr>
<th>
<b>Existing API Name</b></th><th>
<b>Current API Name</b></th><th>
<b>Comments</b></th></tr>
<tr>
<td>
disable</td><td>
disable</td><td>
No Change</td></tr>
<tr>
<td>
enable</td><td>
enable</td><td>
No Change</td></tr>
</table>


