You can easily define your own snippets without any extension. To create or edit your own snippets, select `User Snippets` under `File` > `Preferences` (`Code` > `Preferences` on macOS), and then select the language (by language identifier) for which the snippets should appear, or the New Global Snippets file option if they should appear for all languages. VS Code manages the creation and refreshing of the underlying snippets file(s) for you.

[Create your own snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets)
# Apex

`for`

```java
for (Type variable : ListOrSet) {

}
```

# LWC

## HTML

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

## JS

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
