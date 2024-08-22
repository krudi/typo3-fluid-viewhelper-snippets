### CSS Asset ViewHelper

**Trigger the Snippet:** Type `fAssetCss` in your IDE or editor to trigger this snippet.

**Description:**
Includes a CSS file in TYPO3 templates, identified by a unique identifier.

**Snippet Code:**

```html
<f:asset.css
    identifier="identifier123"
    src="EXT:my_ext/Resources/Public/Css/foo.css"
/>
```

---

### CSS Asset Inline ViewHelper

**Trigger the Snippet:** Type `fAssetCssInline` in your IDE or editor to trigger this snippet.

**Description:**
Includes inline CSS in TYPO3 templates, identified by a unique identifier.

**Snippet Code:**

```html
<f:asset.css identifier="identifier123">
    /* Inline CSS content here */
</f:asset.css>
```

---

### Script Asset ViewHelper

**Trigger the Snippet:** Type `fAssetScript` in your IDE or editor to trigger this snippet.

**Description:**
Includes a JavaScript file in TYPO3 templates, identified by a unique identifier and optionally using a nonce for security.

**Snippet Code:**

```html
<f:asset.script
    identifier="identifier123"
    src="EXT:my_ext/Resources/Public/JavaScript/foo.js"
    useNonce="1"
/>
```

---

### Script Asset ViewHelper

**Trigger the Snippet:** Type `fAssetScriptInline` in your IDE or editor to trigger this snippet.

**Description:**
Includes inline JavaScript in TYPO3 templates, identified by a unique identifier and optionally using a nonce for security.

**Snippet Code:**

```html
<f:asset.script
    identifier="identifier123"
    useNonce="1"
>
    // Inline JavaScript content here
</f:asset.script>
```
