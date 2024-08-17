### Alias ViewHelper

**Trigger the Snippet:** Type `fAlias` in your IDE or editor.

**Description:**
Declares new variables that are aliases of existing variables, simplifying template logic where variables need renaming.

**Snippet Code:**

```html
<f:alias
    map="{${1:x}: '${2:foo}'}"
>
    ${3:${1}}
</f:alias>
```

---

### Case ViewHelper

**Trigger the Snippet:** Type `fCase` in your IDE or editor.

**Description:**
Used within the <f:switch> ViewHelper as a single case. Matches a given value and executes the nested content if the match is successful.

**Snippet Code:**

```html
<f:case
    value="${1}"
>
    ${2}
</f:case>
```

---

### CObject ViewHelper

**Trigger the Snippet:** Type `fCObject` in your IDE or editor.

**Description:**
Renders content objects defined in TypoScript, allowing for integration of complex content structures directly within Fluid templates.
**Snippet Code:**

```html
<f:cObject
    currentValueKey="${1}"
    data="${2}"
    table="${3}"
    typoscriptObjectPath="${4}"
>
    ${5}
</f:cObject>
```

---

### CObject Inline ViewHelper

**Trigger the Snippet:** Type `fCObjectInline` in your IDE or editor.

**Description:**
Inline rendering of TypoScript content objects, particularly useful for embedding TypoScript-driven content in Fluid conditionals or loops.

**Snippet Code:**

```html
{f:cObject(
    currentValueKey: '${1}',
    data: '${2}',
    table: '${3}',
    typoscriptObjectPath: '${4}'
)}
```

---

### Comment ViewHelper

**Trigger the Snippet:** Type `fComment` in your IDE or editor.

**Description:**
Hides content within templates from being rendered, useful for developers to leave notes or deactivate code sections temporarily without removal.

**Snippet Code:**

```html
<f:comment>
    ${1}
</f:comment>
```

---

### Constant ViewHelper

**Trigger the Snippet:** Type `fConstant` in your IDE or editor.

**Description:**
Accesses PHP constants directly within templates, facilitating the use of configuration or environment-specific values.

**Snippet Code:**

```html
<f:constant
    name="${1}"
>
    ${2}
</f:constant>

---

### Count ViewHelper

**Trigger the Snippet:** Type `fCount` in your IDE or editor.

**Description:**
Counts the elements in an array or an object implementing Countable, returning the count as a number.

**Snippet Code:**

```html
<f:count
    subject="${1}"
>
    ${2}
</f:count>
```

---

### Count Inline ViewHelper

**Trigger the Snippet:** Type `fCountInline` in your IDE or editor.

**Description:**
Inline version for quickly obtaining counts of array or Countable objects, useful in loops or conditionals.

**Snippet Code:**

```html
{f:count(
    subject: '${1}'
)}
```

---

### Cycle Inline ViewHelper

**Trigger the Snippet:** Type `fCycleInline` in your IDE or editor.

**Description:**
Inline version of the <f:cycle> ViewHelper, ideal for situations where you need to quickly cycle through values within an expression.

**Snippet Code:**

```html
{f:cycle(
    values: '${1}',
    as: '${2}'
)}
```

---

### Backend Debug ViewHelper

**Trigger the Snippet:** Type `fDebug` in your IDE or editor.

**Description:**
A basic <f:debug> ViewHelper that provides debugging information with a default title "Debug" and includes all variables ({_all}) by default.
**Snippet Code:**

```html
<f:debug
    title="Debug"
>
    ${1:{_all}}
</f:debug>
```

---

### Default Case ViewHelper

**Trigger the Snippet:** Type `fElse` in your IDE or editor.

**Description:**
A ViewHelper that specifies the 'default' case when used within the <f:switch> ViewHelper.

```html
<f:defaultCase>
    ${1}
</f:defaultCase>
```

---

### Else ViewHelper

**Trigger the Snippet:** Type `fElse` in your IDE or editor.

**Description:**
Defines the Else-Branch of a condition. Only effective when used inside an <f:if> block.

```html
<f:else>
    ${1}
</f:else>
```

---

### Feature ViewHelper

**Trigger the Snippet:** Type `fFeature` in your IDE or editor.

**Description:**
Checks if a feature flag is enabled and allows conditional rendering of content based on the feature's state.

```html
<f:feature
    name="${1}"
>
    <f:then>
        ${2}
    </f:then>
    <f:else>
        ${3}
    </f:else>
</f:feature>
```

---

### First ViewHelper

**Trigger the Snippet:** Type `fFirst` in your IDE or editor.

**Description:**
The FirstViewHelper returns the first item of an array, useful when you need to access the initial element in a list.

```html
<f:first
    value="${1}"
>
${2}
</f:first>
```

---

### First Inline ViewHelper

**Trigger the Snippet:** Type `fFirstInline` in your IDE or editor.

**Description:**
Inline version of the <f:first> ViewHelper, allowing quick access to the first element of an array within an expression.

```html
{f:first(
    value: '${1}'
)}

---

### FlashMessages ViewHelper

**Trigger the Snippet:** Type `fFlashMessages` in your IDE or editor.

**Description:**
Renders the flash messages as an unsorted list, useful for displaying user feedback messages.

```html
<f:flashMessages
    as="${1:flashMessages}"
    queueIdentifier="${2:defaultQueue}"
>
    ${3}
</f:flashMessages>
```

---

### FlashMessages Inline ViewHelper

**Trigger the Snippet:** Type `fFlashMessagesInline` in your IDE or editor.

**Description:**
Inline version of the <f:flashMessages> ViewHelper for quick rendering of flash messages.

```html
{f:flashMessages(
    as: '${1:flashMessages}',
    queueIdentifier: '${2:defaultQueue}'
)}
```

---

### For ViewHelper

**Trigger the Snippet:** Type `fFor` in your IDE or editor.

**Description:**
Loop ViewHelper to iterate over arrays, useful for processing collections of items.

```html
<f:for
    each="{${1:array}}"
    as="${2:item}"
    key="${3:key}"
    iteration="${4:iterator}"
    reverse="${5:false}"
>
    ${6}
</f:for>
```

---

### GroupedFor ViewHelper

**Trigger the Snippet:** Type `fGroupedFor` in your IDE or editor.

**Description:**
Grouped loop ViewHelper to iterate over arrays, grouping by a specific property.

```html
<f:groupedFor
    each="{${1:array}}"
    as="${2:item}"
    groupBy="${3:property}"
    groupKey="${4:groupKey}"
>
    ${5}
</f:groupedFor>
```

---

### If ViewHelper

**Trigger the Snippet:** Type `fIf` in your IDE or editor.

**Description:**
Implements a basic if condition, useful for rendering content conditionally.

```html
<f:if
    condition="${1:{condition}}"
>
    ${2}
</f:if>
```

---

### If Inline

**Trigger the Snippet:** Type `fIfInline` in your IDE or editor.

**Description:**
Inline version of the <f:if> ViewHelper for basic conditional rendering.

```html
{f:if(
    condition: '${1:{condition}}'
)}
```

---

### If ViewHelper (with additional conditions)

**Trigger the Snippet:** Type `fIfThenElse` in your IDE or editor.

**Description:**
Implements an if/else condition, useful for branching logic within your templates.

```html
<f:if
    condition="${1:condition}"
>
    <f:then>${2}</f:then>
    <f:else>${3}</f:else>
</f:if>
```

---

### IfThenElse Inline

**Trigger the Snippet:** Type `fIfThenElseInline` in your IDE or editor.

**Description:**
Inline version of the <f:if> ViewHelper with condition, then, and else attributes.

```html
{f:if(
    condition: '${1:{condition} == 1}',
    then: '${2}',
    else: '${3}'
)}
```

---

### Image ViewHelper

**Trigger the Snippet:** Type `fImage` in your IDE or editor.

**Description:**
Resizes a given image and renders the respective img tag with selected attributes.

```html
<f:image
    image="{${1:imageObject}}"
    alt="${2:alt text}"
    width="${3:width}"
    height="${4:height}"
    fileExtension="${5:fileExtension}"
/>
```

---

### Image Inline

**Trigger the Snippet:** Type `fImageInline` in your IDE or editor.

**Description:**
Inline version of the <f:image> ViewHelper with selected attributes, for quick image rendering within expressions.

```html
{f:image(
    image: '{${1:imageObject}}',
    alt: '${2:alt text}',
    width: '${3:width}',
    height: '${4:height}',
    fileExtension: '${5:fileExtension}'
)}
```

---

### Inline ViewHelper

**Trigger the Snippet:** Type `fInline` in your IDE or editor.

**Description:**
Inline Fluid rendering ViewHelper to render Fluid code stored in a variable.

```html
<f:inline
    code="${1:code}"
/>
```

---

### Inline Inline

**Trigger the Snippet:** Type `fInlineInline` in your IDE or editor.

**Description:**
Inline version of the <f:inline> ViewHelper for rendering Fluid code stored in a variable.

```html
{f:inline(
    code: '${1:code}'
)}
```

---

### Join ViewHelper

**Trigger the Snippet:** Type `fJoin` in your IDE or editor.

**Description:**
Combines elements from an array into a single string, useful for creating comma-separated lists or similar structures.

```html
<f:join
    value="{${1:array}}"
    separator="${2:, }"
    separatorLast="${3: and }"
/>
```

---

### Join Inline

**Trigger the Snippet:** Type `fJoinInline` in your IDE or editor.

**Description:**
Inline version of the <f:join> ViewHelper for quick concatenation of array elements into a string.

```html
{f:join(
    value: '{${1:array}}',
    separator: '${2:, }',
    separatorLast: '${3: and }'
)}
```
