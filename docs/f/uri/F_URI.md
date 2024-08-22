### Uri fUriAction ViewHelper

**Trigger the Snippet:** Type `fTransformHtml` in your IDE or editor.

**Description:**
A ViewHelper for creating URIs to Extbase actions. This is useful for generating links that target specific actions within a controller, allowing for dynamic navigation within TYPO3 extensions.

**Snippet Code:**

```html
<f:uri.action
    action="index"
    controller="Default"
    pluginName="MyPlugin"
    extensionName="MyExtension"
    arguments="{arguments}"
>
    URI to action
</f:uri.action>
```

---

### Uri External ViewHelper

**Trigger the Snippet:** Type `fUriExternal` in your IDE or editor.

**Description:**
A ViewHelper for creating URIs to external targets. This is useful for linking to external websites while specifying a default scheme, ensuring consistent URL formats.

**Snippet Code:**

```html
<f:uri.external
    defaultScheme="https"
    uri="https://example.com"
>
    External URI
</f:uri.external>
```

---

### Uri Image ViewHelper

**Trigger the Snippet:** Type `fUriImage` in your IDE or editor.

**Description:**
Resizes a given image (if required) and returns its relative path. This ViewHelper is handy for generating image URLs with various transformations such as resizing and cropping.

**Snippet Code:**

```html
<f:uri.image
    image="{imageObject}"
    alt="Alt text"
    width="800"
    height="auto"
    fileExtension="jpg"
>
    Image URI
</f:uri.image>
```

---

### Uri Page ViewHelper

**Trigger the Snippet:** Type `fUriPage` in your IDE or editor.

**Description:**
A ViewHelper for creating URIs to TYPO3 pages. This snippet is useful for generating internal links to TYPO3 pages, with options to add query strings and customize the URI.

**Snippet Code:**

```html
<f:uri.page
    absolute="false"
    addQueryString="false"
    additionalParams="{additionalParams}"
    argumentsToBeExcludedFromQueryString="{argumentsToExclude}"
    language="0"
    linkAccessRestrictedPages="false"
    noCache="false"
    pageType="0"
    pageUid="1"
    section="section"
>
    Page URI
</f:uri.page>
```

---

### Uri Resource ViewHelper

**Trigger the Snippet:** Type `fUriPage` in your IDE or editor.

**Description:**
A ViewHelper for creating URIs to resources. This is useful for linking to static resources such as images, CSS files, or JavaScript files managed by TYPO3.

**Snippet Code:**

```html
<f:uri.resource
    absolute="false"
    extensionName="MyExtension"
    path="Resources/Public/Images/image.jpg"
    useCacheBusting="true"
>
    Resource URI
</f:uri.resource>
```

---

### Uri Typolink ViewHelper

**Trigger the Snippet:** Type `fUriTypolink` in your IDE or editor.

**Description:**
A ViewHelper to create URIs from fields supported by the link wizard. This is useful for generating complex links using TYPO3's link wizard configuration.

**Snippet Code:**

```html
<f:uri.typolink parameter="1">
    Typolink URI
</f:uri.typolink>
```
