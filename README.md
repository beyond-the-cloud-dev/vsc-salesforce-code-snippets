You can easily define your own snippets without any extension. To create or edit your own snippets, select `User Snippets` under `File` > `Preferences` (`Code` > `Preferences` on macOS), and then select the language (by language identifier) for which the snippets should appear, or the New Global Snippets file option if they should appear for all languages. VS Code manages the creation and refreshing of the underlying snippets file(s) for you.

[Create your own snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets)

To import snippets from this repo, open the linked file for Apex, Html and JavaScript files, and copy their content to your snippet files.

# [Apex](./apex.code-snippets)

| Short version | Regular version |          Description          | Example                                                                                                   |
| :-----------: | :-------------: | :---------------------------: | :-------------------------------------------------------------------------------------------------------- |
|      for      |       for       |         for statement         | for (_Type_ _variable_ : _listOrSet_) { <br>&nbsp;&nbsp;&nbsp;&nbsp;**cursor**<br>},                      |
|     foro      |      foro       | Loop through queried SObjects | for (_Type_ _variable_ : [SELECT _fieldsList_ FROM _Type_) { <br>&nbsp;&nbsp;&nbsp;&nbsp;**cursor**<br>}, |

`for`

```java
for (Type variable : ListOrSet) {

}
```

# LWC

## [HTML](./lwc-html.code-snippets)

`templateForEach`

```js
<template for:each={array} for:item="item"></template>
```

`templateIfFalse`

```js
<template if:false={property}></template>
```

`templateIfTrue`

```js
<template if:true={property}></template>
```

## [JS](./lwc-js.code-snippets)

`constructor`

```js
constructor() {

}
```

`customEvent`

```js
new CustomEvent("eventName", { detail: details });
```

`disconnectedCallback`

```js
disconnectedCallback() {

}
```

`importApexMethod`

```js
import apexMethodName from "@salesforce/apex/Namespace.ClassName.apexMethodReference";
```

`importCustomLabel`

```js
import labelName from "@salesforce/label/labelReference";
```

`importField`

```js
import fieldName from "@salesforce/schema/objectApiName.fieldApiName";
```

`importNavigationMixin`

```js
import { NavigationMixin } from "lightning/navigation";
```

`importObject`

```js
import objectName from "@salesforce/schema/objectApiName";
```

`importUserId`

```js
import userId from "@salesforce/user/Id";
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
