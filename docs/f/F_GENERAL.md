### Alias ViewHelper

**Trigger the Snippet:** Type `fAlias` in your IDE or editor.

**Description:**
Declares new variables that are aliases of existing variables, simplifying template logic where variables need renaming.

**Snippet Code:**

```html
<f:alias map="{${1:x}: '${2:foo}'}">
    ${3:${1}}
</f:alias>
```

---

### Alias Inline ViewHelper

**Trigger the Snippet:** Type `fAliasInline` in your IDE or editor.

**Description:**
The Alias Inline ViewHelper allows you to declare new variables as aliases of other variables within a single line. This is particularly useful for simplifying complex expressions or reusing values in Fluid templates without needing to create a block-level alias.

**Snippet Code:**

```html
{f:alias(map: {${1:x}: '${2:foo}'})}
```

---

### Case ViewHelper

**Trigger the Snippet:** Type `fCase` in your IDE or editor.

**Description:**
Used within the <f:switch> ViewHelper as a single case. Matches a given value and executes the nested content if the match is successful.

**Snippet Code:**

```html
<f:case value="${1}">
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
<f:constant name="${1}">
    ${2}
</f:constant>

---

### Count ViewHelper

**Trigger the Snippet:** Type `fCount` in your IDE or editor.

**Description:**
Counts the elements in an array or an object implementing Countable, returning the count as a number.

**Snippet Code:**

```html
<f:count subject="${1}">
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
{f:count(subject: '${1}')}
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
<f:debug title="Debug"
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
<f:feature name="${1}">
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
<f:first value="${1}">
    ${2}
</f:first>
```

---

### First Inline ViewHelper

**Trigger the Snippet:** Type `fFirstInline` in your IDE or editor.

**Description:**
Inline version of the <f:first> ViewHelper, allowing quick access to the first element of an array within an expression.

```html
{f:first(value: '${1}')}

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
<f:if condition="${1:condition}">
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
{f:if(condition: '${1:{condition} == 1}', then: '${2}', else: '${3}')}
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
<f:inline code="${1:code}" />
```

---

### Inline Inline

**Trigger the Snippet:** Type `fInlineInline` in your IDE or editor.

**Description:**
Inline version of the <f:inline> ViewHelper for rendering Fluid code stored in a variable.

```html
{f:inline(code: '${1:code}')}
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

### Layout ViewHelper

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

### Render ViewHelper

**Trigger the Snippet:** Type `fRender` in your IDE or editor.

**Description:**
Renders a section or partial with specified arguments. This ViewHelper is integral for reusing template parts, ensuring modular and maintainable code. It dynamically includes sections or partials into your templates based on given conditions or arguments.

**Snippet Code:**

```html
<f:render
    section="${1:someSection}"
    partial="${2:partialName}"
    arguments="${3:{_all}}"
/>
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
