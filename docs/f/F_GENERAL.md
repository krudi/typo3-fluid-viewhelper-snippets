### Alias ViewHelper

**Trigger the Snippet:** Type `fAlias` in your IDE or editor.

**Description:**
Declares new variables that are aliases of existing variables, simplifying template logic where variables need renaming.

**Snippet Code:**

```html
<f:alias map="{x: 'foo'}">
    Content using alias
    {x}
</f:alias>
```

---

### Alias Inline ViewHelper

**Trigger the Snippet:** Type `fAliasInline` in your IDE or editor.

**Description:**
The Alias Inline ViewHelper allows you to declare new variables as aliases of other variables within a single line. This is particularly useful for simplifying complex expressions or reusing values in Fluid templates without needing to create a block-level alias.

**Snippet Code:**

```html
{f:alias(map: {x: 'foo'})}
```

---

### Case ViewHelper

**Trigger the Snippet:** Type `fCase` in your IDE or editor.

**Description:**
Used within the <f:switch> ViewHelper as a single case. Matches a given value and executes the nested content if the match is successful.

**Snippet Code:**

```html
<f:case value="1">
    Content for case 1
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
    currentValueKey="key"
    data="{contentObject}"
    table="tt_content"
    typoscriptObjectPath="lib.contentElement"
>
    CObject content
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
    currentValueKey: 'key',
    data: '{contentObject}',
    table: 'tt_content',
    typoscriptObjectPath: 'lib.contentElement'
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
    This is a comment
</f:comment>
```

---

### Constant ViewHelper

**Trigger the Snippet:** Type `fConstant` in your IDE or editor.

**Description:**
Accesses PHP constants directly within templates, facilitating the use of configuration or environment-specific values.

**Snippet Code:**

```html
<f:constant name="TYPO3_MODE" />
```

---

### Count ViewHelper

**Trigger the Snippet:** Type `fCount` in your IDE or editor.

**Description:**
Counts the elements in an array or an object implementing Countable, returning the count as a number.

**Snippet Code:**

```html
<f:count subject="{array}">
    Counted items: {subject}
</f:count>
```

---

### Count Inline ViewHelper

**Trigger the Snippet:** Type `fCountInline` in your IDE or editor.

**Description:**
Inline version for quickly obtaining counts of array or Countable objects, useful in loops or conditionals.

**Snippet Code:**

```html
{f:count(subject: '{array}')}
```

---

### Cycle ViewHelper

**Trigger the Snippet:** Type `fCycle` in your IDE or editor.

**Description:**
This ViewHelper cycles through the specified values.

**Snippet Code:**

```html
<f:cycle values="{0,1,2}" as="item">
    Item: {item}
</f:cycle>
```

---

### Cycle Inline ViewHelper

**Trigger the Snippet:** Type `fCycleInline` in your IDE or editor.

**Description:**
Inline version of the <f:cycle> ViewHelper, ideal for situations where you need to quickly cycle through values within an expression.

**Snippet Code:**

```html
{f:cycle(
    values: '{0,1,2}',
    as: 'item'
)}
```

---

### Backend Debug ViewHelper

**Trigger the Snippet:** Type `fDebug` in your IDE or editor.

**Description:**
A basic <f:debug> ViewHelper that provides debugging information with a default title "Debug" and includes all variables ({_all}) by default.
**Snippet Code:**

```html
<f:debug title="Debug">{_all}</f:debug>
```

---

### Default Case ViewHelper

**Trigger the Snippet:** Type `fElse` in your IDE or editor.

**Description:**
A ViewHelper that specifies the 'default' case when used within the <f:switch> ViewHelper.

```html
<f:defaultCase>
    Default Content
</f:defaultCase>
```

---

### Else ViewHelper

**Trigger the Snippet:** Type `fElse` in your IDE or editor.

**Description:**
Defines the Else-Branch of a condition. Only effective when used inside an <f:if> block.

```html
<f:else>
    Else Content
</f:else>
```

---

### Feature ViewHelper

**Trigger the Snippet:** Type `fFeature` in your IDE or editor.

**Description:**
Checks if a feature flag is enabled and allows conditional rendering of content based on the feature's state.

```html
<f:feature name="featureFlag">
    <f:then>
        Feature Enabled
    </f:then>
    <f:else>
        Feature Disabled
    </f:else>
</f:feature>
```

---

### First ViewHelper

**Trigger the Snippet:** Type `fFirst` in your IDE or editor.

**Description:**
The FirstViewHelper returns the first item of an array, useful when you need to access the initial element in a list.

```html
<f:first value="{array}">
    First item: {value}
</f:first>
```

---

### First Inline ViewHelper

**Trigger the Snippet:** Type `fFirstInline` in your IDE or editor.

**Description:**
Inline version of the <f:first> ViewHelper, allowing quick access to the first element of an array within an expression.

```html
{f:first(value: '{array}')}
```

---

### FlashMessages ViewHelper

**Trigger the Snippet:** Type `fFlashMessages` in your IDE or editor.

**Description:**
Renders the flash messages as an unsorted list, useful for displaying user feedback messages.

```html
<f:flashMessages
    as="flashMessages"
    queueIdentifier="default"
>
    Flash Messages: {flashMessages}
</f:flashMessages>
```

---

### FlashMessages Inline ViewHelper

**Trigger the Snippet:** Type `fFlashMessagesInline` in your IDE or editor.

**Description:**
Inline version of the <f:flashMessages> ViewHelper for quick rendering of flash messages.

```html
{f:flashMessages(
    as: 'flashMessages',
    queueIdentifier: 'default'
)}
```

---

### For ViewHelper

**Trigger the Snippet:** Type `fFor` in your IDE or editor.

**Description:**
Loop ViewHelper to iterate over arrays, useful for processing collections of items.

```html
<f:for
    each="{items}"
    as="item"
    key="key"
    iteration="iteration"
    reverse="false"
>
    Item: {item}, Key: {key}, Iteration: {iteration}
</f:for>
```

---

### GroupedFor ViewHelper

**Trigger the Snippet:** Type `fGroupedFor` in your IDE or editor.

**Description:**
Grouped loop ViewHelper to iterate over arrays, grouping by a specific property.

```html
<f:groupedFor
    each="{items}"
    as="group"
    groupBy="property"
    groupKey="groupKey"
>
    Group: {group}, Group Key: {groupKey}
</f:groupedFor>
```

---

### If ViewHelper

**Trigger the Snippet:** Type `fIf` in your IDE or editor.

**Description:**
Implements a basic if condition, useful for rendering content conditionally.

```html
<f:if condition="{condition}">
    Content if true
</f:if>
```

---

### If Inline

**Trigger the Snippet:** Type `fIfInline` in your IDE or editor.

**Description:**
Inline version of the <f:if> ViewHelper for basic conditional rendering.

```html
{f:if(condition: '{condition}', then: 'Content if true', else: 'Content if false')}
```

---

### If ViewHelper (with additional conditions)

**Trigger the Snippet:** Type `fIfThenElse` in your IDE or editor.

**Description:**
Implements an if/else condition, useful for branching logic within your templates.

```html
<f:if condition="{condition}">
    <f:then>
        Content if true
    </f:then>
    <f:else>
        Content if false
    </f:else>
</f:if>
```

---

### IfThenElse Inline

**Trigger the Snippet:** Type `fIfThenElseInline` in your IDE or editor.

**Description:**
Inline version of the <f:if> ViewHelper with condition, then, and else attributes.

```html
{f:if(condition: '{condition}', then: 'Content if true', else: 'Content if false')}
```

---

### Image ViewHelper

**Trigger the Snippet:** Type `fImage` in your IDE or editor.

**Description:**
Resizes a given image and renders the respective img tag with selected attributes.

```html
<f:image
    image="{imageObject}"
    alt="alt text"
    width="800"
    height="auto"
    fileExtension="jpg"
/>
```

---

### Image Inline

**Trigger the Snippet:** Type `fImageInline` in your IDE or editor.

**Description:**
Inline version of the <f:image> ViewHelper with selected attributes, for quick image rendering within expressions.

```html
{f:image(
    image: '{imageObject}',
    alt: 'alt text',
    width: '800',
    height: 'auto',
    fileExtension: 'jpg'
)}
```

---

### Inline ViewHelper

**Trigger the Snippet:** Type `fInline` in your IDE or editor.

**Description:**
Inline Fluid rendering ViewHelper to render Fluid code stored in a variable.

```html
<f:inline code="someFluidCode" />
```

---

### Inline Inline

**Trigger the Snippet:** Type `fInlineInline` in your IDE or editor.

**Description:**
Inline version of the <f:inline> ViewHelper for rendering Fluid code stored in a variable.

```html
{f:inline(code: 'someFluidCode')}
```

---

### Join ViewHelper

**Trigger the Snippet:** Type `fJoin` in your IDE or editor.

**Description:**
Combines elements from an array into a single string, useful for creating comma-separated lists or similar structures.

```html
<f:join
    value="{array}"
    separator=", "
    separatorLast=" and "
/>
```

---

### Join Inline

**Trigger the Snippet:** Type `fJoinInline` in your IDE or editor.

**Description:**
Inline version of the <f:join> ViewHelper for quick concatenation of array elements into a string.

```html
{f:join(value: '{array}', separator: ', ', separatorLast: ' and ')}
```

---

### Last ViewHelper

**Trigger the Snippet:** Type `fLast` in your IDE or editor.

**Description:**
Returns the last item of an array. This ViewHelper is useful for extracting the final element from a list.

**Snippet Code:**

```html
<f:last value="{array}" />
```

---

### Layout ViewHelper

**Trigger the Snippet:** Type `fLayout` in your IDE or editor.

**Description:**
Selects a layout to be used for the current template. This is essential for setting up the overall structure of your TYPO3 templates.

**Snippet Code:**

```html
<f:layout name="main" />
```

---

### Media ViewHelper

**Trigger the Snippet:** Type `fMedia` in your IDE or editor.

**Description:**
Renders a given media file with the correct HTML tag. This ViewHelper is particularly useful for embedding media files like videos and audio in your templates.

**Snippet Code:**

```html
<f:media
    file="{file}"
    width="400"
     height="375"
     additionalConfig="{
        loop: '1',
        autoplay: '1'
    }"
/>
```

---

### Or ViewHelper

**Trigger the Snippet:** Type `fOr` in your IDE or editor.

**Description:**
Use alternative text if content is null. This is useful for providing fallback values when dealing with potentially undefined variables.

**Snippet Code:**

```html
{undefinedVariable -> f:or(alternative='fallback')}
```

---

### Render ViewHelper

**Trigger the Snippet:** Type `fRender` in your IDE or editor.

**Description:**
Renders a section or partial with specified arguments. This ViewHelper is integral for reusing template parts, ensuring modular and maintainable code. It dynamically includes sections or partials into your templates based on given conditions or arguments.

**Snippet Code:**

```html
<f:render
    section="someSection"
    partial="partialName"
    arguments="{_all}"
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
    value="Hello World"
    search="World"
    replace="Fluid"
/>
```

---

### Section ViewHelper

**Trigger the Snippet:** Type `fSection` in your IDE or editor.

**Description:**
Declares sections in templates for later use. Sections are useful for organizing and reusing template content.

**Snippet Code:**

```html
<f:section name="sectionName">
    This is a section.
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
    HTML content without spaces between tags
</f:spaceless>
```

---

### Split ViewHelper

**Trigger the Snippet:** Type `fSplit` in your IDE or editor.

**Description:**
Splits a string by the specified separator. This ViewHelper is useful for breaking strings into arrays based on a delimiter.

**Snippet Code:**

```html
<f:split value="1,5,8" separator="," limit="2" />
```

---

### Switch ViewHelper

**Trigger the Snippet:** Type `fSplit` in your IDE or editor.

**Description:**
Switches content based on the value or expression. This ViewHelper is useful for handling multiple conditional cases in your templates.

**Snippet Code:**

```html
<f:switch expression="{person.gender}">
    <f:case value="male">Mr.</f:case>
    <f:case value="female">Mrs.</f:case>
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
    Content if condition is true
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
    key="LLL:EXT:my_ext/Resources/Private/Language/locallang.xlf:key" extensionName="my_ext"
    arguments="{
        0: 'dog',
        1: 'fox'
    }"
    default="default value"
/>
```

---

### Translate Inline ViewHelper

**Trigger the Snippet:** Type `fTranslateInline` in your IDE or editor.

**Description:**
Translates a key inline from a locallang or custom locallang file. This is useful for embedding translations directly inside a text string within a Fluid template.

**Snippet Code:**

```html
{f:translate(
    key: 'LLL:EXT:my_ext/Resources/Private/Language/locallang.xlf:key',
    extensionName: 'my_ext'
)}
```

---

### Translate Inline ViewHelper (with additional conditions)

**Trigger the Snippet:** Type `fTranslateArgumentsInline` in your IDE or editor.

**Description:**
Translates a key inline from a locallang or custom locallang file with additional options like arguments and default fallback text. This is useful when your translation involves dynamic placeholders.

**Snippet Code:**

```html
{f:translate(
    key: 'LLL:EXT:my_ext/Resources/Private/Language/locallang.xlf:key',
    extensionName: 'my_ext',
    arguments: {
        0: 'dog',
        1: 'fox'
    },
    default: 'Default translation'
)}
```

---

### Variable ViewHelper

**Trigger the Snippet:** Type `fVariable` in your IDE or editor.

**Description:**
Assigns a template variable. This ViewHelper is useful for setting variables within your templates that can be used later in the rendering process.

**Snippet Code:**

```html
<f:variable name="myVariable">
    Variable content
</f:variable>
```
