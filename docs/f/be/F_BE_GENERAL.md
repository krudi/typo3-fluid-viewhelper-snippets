### Backend Infobox ViewHelper

**Trigger the Snippet:** Type `fBeInfobox` in your IDE or editor to trigger this snippet.

**Description:**
Renders a styled content infobox in the backend with various states.

**Snippet Code:**

```html
<f:be.infobox title="Information"
    message="This is an info message."
    state="0"
    iconName="actions-info"
    disableIcon="false"
>
    Additional content here.
</f:be.infobox>
```

---

### Backend Link ViewHelper

**Trigger the Snippet:** Type `fBeLink` in your IDE or editor to trigger this snippet.

**Description:**
Creates URIs to backend modules.

**Snippet Code:**

```html
<f:be.link route="moduleName"
    parameters="{}"
    referenceType="absolute"
    additionalAttributes="{}"
    aria="{}"
    data="{}"
>
    Link Text
</f:be.link>
```

---

### Backend PageRenderer ViewHelper

**Trigger the Snippet:** Type `fBePageRenderer` in your IDE or editor to trigger this snippet.

**Description:**
Registers backend module resources like CSS and JavaScript using the PageRenderer.

**Snippet Code:**

```html
<f:be.pageRenderer
    pageTitle="My Module"
    includeCssFiles="['EXT:my_extension/Resources/Public/Css/style.css']"
    includeJsFiles="['EXT:my_extension/Resources/Public/JavaScript/script.js']"
    addJsInlineLabels="{}"
    includeJavaScriptModules="[]"
    addInlineSettings="{}"
/>
```

---

### Backend TableList ViewHelper

**Trigger the Snippet:** Type `fBeTableList` in your IDE or editor to trigger this snippet.

**Description:**
Renders a record list as known from the TYPO3 list module.

**Snippet Code:**

```html
<f:be.tableList tableName="tt_content"
    fieldList="['uid', 'header', 'bodytext']"
    storagePid="1"
    levels="0"
    filter=""
    recordsPerPage="10"
    sortField="sorting"
    sortDescending="false"
    readOnly="false"
    enableClickMenu="true"
    enableControlPanels="true"
    clickTitleMode="edit"
/>
```

---

### Backend Uri ViewHelper

**Trigger the Snippet:** Type `fBeUri` in your IDE or editor to trigger this snippet.

**Description:**
Creates URIs to backend modules.

**Snippet Code:**

```html
<f:be.uri route="moduleName"
    parameters="{}"
    referenceType="absolute"
/>
```
