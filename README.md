You can easily define your own snippets without any extension. To create or edit your own snippets, select `User Snippets` under `File` > `Preferences` (`Code` > `Preferences` on macOS), and then select the language (by language identifier) for which the snippets should appear, or the New Global Snippets file option if they should appear for all languages. VS Code manages the creation and refreshing of the underlying snippets file(s) for you.

[Create your own snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets)
# Apex

`for`

```java
for (Type variable : ListOrSet) {

}
```

# LWC

`CustomEvent`

```js
new CustomEvent('eventName', { detail: details });
```

`ShowToastEvent`

```js
new ShowToastEvent({ 'title', 'message', 'variant' });
```

`importApexMethod`

```js
import apexMethodName from '@salesforce/apex/Namespace.ClassName.apexMethodReference';
```

`importCustomLabel`

```js
import labelName from '@salesforce/label/labelReference';
``
