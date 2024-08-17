### Uri fUriAction ViewHelper

**Trigger the Snippet:** Type `fTransformHtml` in your IDE or editor.

**Description:**
A ViewHelper for creating URIs to Extbase actions. This is useful for generating links that target specific actions within a controller, allowing for dynamic navigation within TYPO3 extensions.

**Snippet Code:**

```html
<f:uri.action
    action="${1}"
    controller="${2}"
    pluginName="${3}"
    extensionName="${4}"
    arguments="${5:array}"
>
    ${6}
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
    defaultScheme="${1:https}"
    uri="${2}"
>
    ${3}
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
    image="{${1:imageObject}}"
    alt="${2:alt text}"
    width="${3:width}"
    height="${4:height}"
    fileExtension="${5:fileExtension}"
>
    ${6}
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
    absolute="${1:false}"
    addQueryString="${2:false}"
    additionalParams="${3:array}"
    argumentsToBeExcludedFromQueryString="${4:array}"
    language="${5}"
    linkAccessRestrictedPages="${6:false}"
    noCache="${7:false}"
    pageType="${8:0}"
    pageUid="${9}"
    section="${10}"
>
    ${11}
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
    absolute="${1:false}"
    extensionName="${2}"
    path="${3}"
    useCacheBusting="${4:true}"
>
    ${5}
</f:uri.resource>
```

---

### Uri Typolink ViewHelper

**Trigger the Snippet:** Type `fUriTypolink` in your IDE or editor.

**Description:**
A ViewHelper to create URIs from fields supported by the link wizard. This is useful for generating complex links using TYPO3's link wizard configuration.

**Snippet Code:**

```html
<f:uri.typolink parameter="${6}">
    ${10}
</f:uri.typolink>
```
