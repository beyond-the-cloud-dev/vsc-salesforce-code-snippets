# Salesforce Snippets

## Features

# [Apex](./apex.code-snippets)

| Short version | Regular version |          Description          | Example                                                                                                  |
| :-----------: | :-------------: | :---------------------------: | :------------------------------------------------------------------------------------------------------- |
|      for      |       for       |         for statement         | for (_Type_ _variable_ : _listOrSet_) { <br>&nbsp;&nbsp;&nbsp;&nbsp;**cursor**<br>},                     |
|     foro      |      foro       | Loop through queried SObjects | for (_Type_ _variable_ : [SELECT _fieldsList_ FROM _Type_) { <br>&nbsp;&nbsp;&nbsp;&nbsp;**cursor**<br>} |

# LWC

## [HTML](./lwc-html.code-snippets)

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
</table>

## [JS](./lwc-js.code-snippets)
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
<td> renderedCallback </td>
<td>

```js
initialRender = true;
renderedCallback() {
    if (this.initialRender) {
        // Your code here.
        this.initialRender = false;
    }
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
