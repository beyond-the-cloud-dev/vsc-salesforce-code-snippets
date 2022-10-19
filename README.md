# Salesforce Snippets
## List of Snippets
[![Apex](https://img.shields.io/badge/Apex-11-green?style=flat-square)](#apex)
[![LWC-HTML](https://img.shields.io/badge/LWC_HTML-13-yellow?style=flat-square)](#html)
[![LWC-JS](https://img.shields.io/badge/LWC_JavaScript-25-blue?style=flat-square)](#js)
## Features

# [Apex](./snippets/apex.json)

<table>
<tr>
<td> Prefix </td>
<td> Example </td>
</tr>
<tr>
<td>foro</td>
<td>

```java
for (Type variable : [SELECT fieldsList FROM Type) {
    //Your code here
}
```

</td>
</tr>

<tr>
<td>inst</td>
<td>

```java
if (objects[0] instanceof Account) {
    Account acc = (Account) objects[0];
}
```

</td>
</tr>

<tr>
<td>sa</td>
<td>

```java
System.assert();
```

</td>
</tr>

</tr>

<tr>
<td>saf</td>
<td>

```java
System.assert(false, );
```

</td>
</tr>

<tr>
<td>sae</td>
<td>

```java
System.assertEquals(expected, actual);
```

</td>
</tr>

<tr>
<td>san</td>
<td>

```java
System.assertEquals(null, );
```

</td>
</tr>

<tr>
<td>sane</td>
<td>

```java
System.assertNotEquals(expected, actual);
```

</td>
</tr>

<tr>
<td>sann</td>
<td>

```java
System.assertNotEquals(null, );
```

</td>
</tr>

<tr>
<td>sd</td>
<td>

```java
System.debug(LoggingLevel.DEBUG, 'your message here: ' + variableHere);
```

</td>
</tr>

<tr>
<td>sdp</td>
<td>

```java
System.debug(LoggingLevel.DEBUG, 'your message here: ' + JSON.SerializePretty(objectVariable));
```

</td>
</tr>

<tr>
<td>sra</td>
<td>

```java
System.runAs(user) {
    //your code here
}
```

</td>
</tr>

</table>


# LWC

## [HTML](./snippets/lwc-html.json)

<table>
<tr>
<td> Prefix </td>
<td> Example </td>
</tr>
<tr>
<td> lightning-button </td>
<td>

```html
<lightning-button variant='base' label='label' title='title' onclick={handleOnClick} class='cssClass'>
</lightning-button>
```
</td>
</tr>
<tr>
<td> lightning-combobox </td>
<td>

```html
<lightning-combobox
    name='name'
    label='label'
    value={value}
    placeholder='placeholder'
    options={options}
    onchange={handleChange}
></lightning-combobox>
```
</td>
</tr>
<tr>
<td> lightning-datatable </td>
<td>

```html
<lightning-datatable
    key-field='Id'
    data={data}
    columns={columns}
    hide-checkbox-column
></lightning-datatable>
```
</td>
</tr>
<tr>
<td> lightning-icon </td>
<td>

```html
<lightning-icon icon-name='iconName' alternative-text='alternativeText' title='title'>
</lightning-icon>
```
</td>
</tr>
<tr>
<td> lightning-input </td>
<td>

```html
<lightning-input type='type' label='label' onchange='handleOnChange'>
</lightning-input>
```
</td>
</tr>
<tr>
<td> lightning-layout </td>
<td>

```html
<lightning-layout horizontal-align='horiznotalAlign' vertical-align='verticalAlign' multiple-rows='multipleRows'>
    <lightning-layout-item padding='around-small'>
    </lightning-layout-item>
    <lightning-layout-item padding='around-small'>
    </lightning-layout-item>
    <lightning-layout-item padding='around-small'>
    </lightning-layout-item>
</lightning-layout>
```
</td>
</tr>
<tr>
<td> lightning-layout-item </td>
<td>

```html
<lightning-layout-item size='size' small-device-size='smallDeviceSize' medium-device-size='mediumDeviceSize' large-device-size='largeDeviceSize' padding='around-small'>
</lightning-layout-item>
```
</td>
</tr>
<tr>
<td> lightning-spinner </td>
<td>

```html
<lightning-spinner alternative-text='alternativeText' size='size'>
</lightning-spinner>
```
</td>
</tr>
<tr>
<td> slot </td>
<td>

```html
<slot name='name'>
</slot>
```
</td>
</tr>
<tr>
<td> templateForEach </td>
<td>

```html
<template for:each={array} for:item='item'>
</template>
```
</td>
</tr>
<tr>
<td> templateIfFalse </td>
<td>

```html
<template if:false={property}>
</template>
```
</td>
</tr>
<tr>
<td> templateIfTrue </td>
<td>

```html
<template if:true={property}>
</template>
```
</td>
</tr>
<tr>
<td> templateIteratorIt </td>
<td>

```html
<template iterator:it={array}>
    <div key={it.value.Id}>
    <div if:true={it.first}></div>
    {it.value.Name}
    <div if:true={it.last}></div>
    </div>
</template>
```
</td>
</tr>
</table>

## [JS](./snippets/lwc-js.json)
<table>
<tr>
<td> Prefix </td>
<td> Example </td>
</tr>
<tr>
<td> asyncAwait </td>
<td>

```js
try {
    const result = await apexMethodName({ apexMethodParams });
} catch (error) {
    console.error(error)
}
```
</td>
</tr>
<tr>
<td> constructor </td>
<td>

```js
constructor() {

}
```
</td>
</tr>
</tr>
<tr>
<td> customEvent </td>
<td>

```js
new CustomEvent('eventName', {
    detail: details,
    bubbles: false,
    composed: false
});
```
</td>
</tr>
<tr>
<td> disconnectedCallback </td>
<td>

```js
disconnectedCallback() {

}
```
</td>
</tr>
<tr>
<td> dispatchEvent </td>
<td>

```js
this.dispatchEvent(customEvent);
```
</td>
</tr>
<tr>
<td> errorCallback </td>
<td>

```js
errorCallback(error, stack) {

}
```
</td>
</tr>
<tr>
<td> getObjectInfo </td>
<td>

```js
import { getObjectInfo } from 'lightning/uiObjectInfoApi';
import objectName from '@salesforce/schema/objectApiName';

@wire(getObjectInfo, { objectApiName: objectName })
propertyOrFunction;
```
</td>
</tr>
<tr>
<td> getPicklistValues </td>
<td>

```js
import { getPicklistValues } from 'lightning/uiObjectInfoApi';
import fieldName from '@salesforce/schema/objectApiName.fieldApiName';

@wire(getPicklistValues, { recordTypeId: '012000000000000AAA', fieldApiName: fieldName })
propertyOrFunction;
```
</td>
</tr>
<tr>
<td> getRecord </td>
<td>

```js
import { getRecord } from 'lightning/uiRecordApi';

@wire(getRecord, { recordId: 'recordId', fields: fields })
propertyOrFunction;
```
</td>
</tr>
<tr>
<td> getRecords </td>
<td>

```js
import { getRecords } from 'lightning/uiRecordApi';

@wire(getRecords, { records: [ { recordIds: 'recordIds', fields: fields } ] })
propertyOrFunction;
```
</td>
</tr>
<tr>
<td> importApexMethod </td>
<td>

```js
import apexMethodName from '@salesforce/apex/Namespace.ClassName.apexMethodReference';
```
</td>
</tr>
<tr>
<td> importField </td>
<td>

```js
import fieldName from '@salesforce/schema/objectApiName.fieldApiName';
```
</td>
</tr>
<tr>
<td> importHasPermission </td>
<td>

```js
import hasPermissionName from '@salesforce/userPermission/PermissionName';
```
</td>
</tr>
<tr>
<td> importNavigationMixin </td>
<td>

```js
import { NavigationMixin } from 'lightning/navigation';
```
</td>
</tr>
<tr>
<td> importObject </td>
<td>

```js
import objectName from '@salesforce/schema/objectApiName';
```
</td>
</tr>
<tr>
<td> importUserId </td>
<td>

```js
import userId from '@salesforce/user/Id';
```
</td>
</tr>
<tr>
<td> querySelector </td>
<td>

```js
this.template.querySelector('element');
```
</td>
</tr>
<tr>
<td> querySelectorAll </td>
<td>

```js
this.template.querySelectorAll('element');
```
</td>
</tr>
<tr>
<td> render </td>
<td>

```js
render() {

}
```
</td>
</tr>
<tr>
<td> renderedCallback </td>
<td>

```js
initialRender = true;
renderedCallback() {
    if (!this.initialRender) {
        return;
    }
    // Your code here.
    this.initialRender = false;
}
```
</td>
</tr>
<tr>
<td> ShowToastEvent </td>
<td>

```js
import { ShowToastEvent } from 'lightning/platformShowToastEvent';
new ShowToastEvent({ 'title', 'message', 'variant' });
```
</td>
</tr>
<tr>
<td> importStaticResource </td>
<td>

```js
import resourceName from '@salesforce/resourceUrl/resourceName';
```
</td>
</tr>
<tr>
<td> thenCatch </td>
<td>

```js
apexMethodName({ apexMethodParams })
.then(result => {

})
.catch(error => {
    console.error(error)
});
```
</td>
</tr>
<tr>
<td> wireMethod </td>
<td>

```js
@wire(apexMethodName, { apexMethodParams })
wiredName({ error, data }) {
    if (data) {

    } else if (error) {
        console.error(error);
    }
}
```
</td>
</tr>
<tr>
<td> wireProperty </td>
<td>

```js
@wire(apexMethodName, { apexMethodParams })
property;
```
</td>
</tr>
</table>

## Release Notes

### 0.0.1
Initial release of Salesforce Snippets.
