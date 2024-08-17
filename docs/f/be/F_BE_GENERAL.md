### Backend Infobox Tag

**Trigger the Snippet:** Type `fBeInfobox` in your IDE or editor to trigger this snippet.

**Description:**
Renders a styled content infobox in the backend with various states.

**Snippet Code:**

```html
<f:be.infobox title="$1"
    message="$2"
    state="${3:-2}"
    iconName="${4}"
    disableIcon="${5:false}">
    $6
</f:be.infobox>
```

---

### Backend Link Tag

**Trigger the Snippet:** Type `fBeLink` in your IDE or editor to trigger this snippet.

**Description:**
Creates URIs to backend modules.

**Snippet Code:**

```html
<f:be.link route="$1"
    parameters="${2:array}"
    referenceType="${3:'absolute'}"
    additionalAttributes="${4:array}"
    aria="${5:array}"
    data="${6:array}">
    $7
</f:be.link>
```

---

### Backend PageRenderer Tag

**Trigger the Snippet:** Type `fBePageRenderer` in your IDE or editor to trigger this snippet.

**Description:**
Registers backend module resources like CSS and JavaScript using the PageRenderer.

**Snippet Code:**

```html
<f:be.pageRenderer
    pageTitle="$1"
    includeCssFiles="${2:array}"
    includeJsFiles="${3:array}"
    addJsInlineLabels="${4:array}"
    includeJavaScriptModules="${5:array}"
    addInlineSettings="${6:array}"
/>
```

---

### Backend TableList Tag

**Trigger the Snippet:** Type `fBeTableList` in your IDE or editor to trigger this snippet.

**Description:**
Renders a record list as known from the TYPO3 list module.

**Snippet Code:**

```html
<f:be.tableList tableName="$1"
    fieldList="${2:array}"
    storagePid="${3:1}"
    levels="${4:0}"
    filter="$5"
    recordsPerPage="${6:0}"
    sortField="$7"
    sortDescending="${8:false}"
    readOnly="${9:false}"
    enableClickMenu="${10:true}"
    enableControlPanels="${11:false}"
    clickTitleMode="${12}"
/>
```

---

### Backend Uri Tag

**Trigger the Snippet:** Type `fBeUri` in your IDE or editor to trigger this snippet.

**Description:**
Creates URIs to backend modules.

**Snippet Code:**

```html
<f:be.uri route="$1"
    parameters="${2:array}"
    referenceType="${3:'absolute'}"
/>
```
