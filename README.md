# salesforce-snippets README

## Features

# [Apex](./apex.code-snippets)

`for`

```java
for (Type variable : ListOrSet) {

}
```

# LWC

## [HTML](./lwc-html.code-snippets)

`templateForEach`

```js
<template for:each={array} for:item='item'>
</template>
```

`templateIfFalse`

```js
<template if:false={property}>
</template>
```

`templateIfTrue`

```js
<template if:true={property}>
</template>
```

## [JS](./lwc-js.code-snippets)

`constructor`

```js
constructor() {

}
```

`customEvent`

```js
new CustomEvent('eventName', { detail: details });
```

`disconnectedCallback`

```js
disconnectedCallback() {

}
```

`importApexMethod`

```js
import apexMethodName from '@salesforce/apex/Namespace.ClassName.apexMethodReference';
```

`importCustomLabel`

```js
import labelName from '@salesforce/label/labelReference';
```

`importField`

```js
import fieldName from '@salesforce/schema/objectApiName.fieldApiName';
```

`importNavigationMixin`

```js
import { NavigationMixin } from 'lightning/navigation';
```

`importObject`

```js
import objectName from '@salesforce/schema/objectApiName';
```

`importUserId`

```js
import userId from '@salesforce/user/Id';
```

`renderedCallback`

```js
initialRender = true;
renderedCallback() {
    if (this.initialRender) {
        this.initialRender = false;
    }
}
```

`ShowToastEvent`

```js
import { ShowToastEvent } from 'lightning/platformShowToastEvent';
new ShowToastEvent({ 'title', 'message', 'variant' });
```

`wireMethod`

```js
import apexMethodName from '@salesforce/apex/Namespace.Classname.apexMethodReference';
@wire(apexMethodName, { apexMethodParams })
wiredName({ error, data }) {
    if (data) {

    } else if (error) {
        console.error(error);
    }
}
```

`wireProperty`

```js
import apexMethodName from '@salesforce/apex/Namespace.Classname.apexMethodReference';
@wire(apexMethodName, { apexMethodParams })
property;
```

## Release Notes

### 0.0.1
Initial release of Salesforce Snippets.
