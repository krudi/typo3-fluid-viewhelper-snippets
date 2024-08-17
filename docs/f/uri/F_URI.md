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

---

### Last ViewHelper

**Trigger the Snippet:** Type `fLast` in your IDE or editor.

**Description:**
Returns the last item of an array. This ViewHelper is useful for extracting the final element from a list.

**Snippet Code:**

```html
<f:last value="{${1:0: 'first', 1: 'second'}}" />
```

---

### Last ViewHelper

**Trigger the Snippet:** Type `fLayout` in your IDE or editor.

**Description:**
Selects a layout to be used for the current template. This is essential for setting up the overall structure of your TYPO3 templates.

**Snippet Code:**

```html
<f:layout name="${1:main}" />
```

---

### Media ViewHelper

**Trigger the Snippet:** Type `fMedia` in your IDE or editor.

**Description:**
Renders a given media file with the correct HTML tag. This ViewHelper is particularly useful for embedding media files like videos and audio in your templates.

**Snippet Code:**

```html
<f:media
    file="{${1:file}}"
    width="${2:400}"
    height="${3:375}"
    ${4:additionalConfig="{loop: '1', autoplay: '1'}"}
/>
```

---

### Or ViewHelper

**Trigger the Snippet:** Type `fOr` in your IDE or editor.

**Description:**
Use alternative text if content is null. This is useful for providing fallback values when dealing with potentially undefined variables.

**Snippet Code:**

```html
{${1:undefinedVariable} -> f:or(alternative=${2:fallback})}
```

---

### Replace ViewHelper

**Trigger the Snippet:** Type `fReplace` in your IDE or editor.

**Description:**
Replaces one or multiple strings with other strings. This ViewHelper is useful for performing text replacements within your templates.

**Snippet Code:**

```html
<f:replace
    value="${1:Hello World}"
    search="${2:World}"
    replace="${3:Fluid}"
/>
```

---

### Section ViewHelper

**Trigger the Snippet:** Type `fSection` in your IDE or editor.

**Description:**
Declares sections in templates for later use. Sections are useful for organizing and reusing template content.

**Snippet Code:**

```html
<f:section
    name="${1:sectionName}"
>
    ${2:This is a section.}
</f:section>
```

---

### Spaceless ViewHelper

**Trigger the Snippet:** Type `fSpaceless` in your IDE or editor.

**Description:**
Removes redundant spaces between HTML tags. This ViewHelper is helpful for minimizing the output HTML by removing unnecessary whitespace.

**Snippet Code:**

```html
<f:spaceless>
    ${1:<div><div><div>text\n\ntext</div></div></div>}
</f:spaceless>
```

---

### Split ViewHelper

**Trigger the Snippet:** Type `fSplit` in your IDE or editor.

**Description:**
Splits a string by the specified separator. This ViewHelper is useful for breaking strings into arrays based on a delimiter.

**Snippet Code:**

```html
<f:split value="${1:1,5,8}" separator="${2:,}" limit="${3:2}" />
```

---

### Switch ViewHelper

**Trigger the Snippet:** Type `fSplit` in your IDE or editor.

**Description:**
Switches content based on the value or expression. This ViewHelper is useful for handling multiple conditional cases in your templates.

**Snippet Code:**

```html
<f:switch
    expression="{${1:person.gender}}"
>
    <f:case value="${2:male}">Mr.</f:case>
    <f:case value="${3:female}">Mrs.</f:case>
    <f:defaultCase>Mr. / Mrs.</f:defaultCase>
</f:switch>
```

---

### Then ViewHelper

**Trigger the Snippet:** Type `fThen` in your IDE or editor.

**Description:**
Used within <f:if> to specify what should be rendered if the condition is true. This ViewHelper defines the content for the true branch of a conditional statement.

**Snippet Code:**

```html
<f:then>
    ${1:content}
</f:then>
```

---

### Translate ViewHelper

**Trigger the Snippet:** Type `fTranslate` in your IDE or editor.

**Description:**
Translates a key from locallang or custom locallang file. This ViewHelper is essential for multilingual TYPO3 websites, allowing for dynamic text translation.

**Snippet Code:**

```html
<f:translate
    key="${1:key1}"
    extensionName="${2:MyExt}"
    ${3:arguments=${4:{0: 'dog', 1: 'fox'}}
    default="${5:default value}}"
/>
```

---

### Variable ViewHelper

**Trigger the Snippet:** Type `fVariable` in your IDE or editor.

**Description:**
Assigns a template variable. This ViewHelper is useful for setting variables within your templates that can be used later in the rendering process.

**Snippet Code:**

```html
<f:variable
    name="${1:myvariable}"
    value="${2:some value}"
/>
```
