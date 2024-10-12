### Translate ViewHelper (ContentBlocks)

**Trigger the Snippet:** Type `cbTranslate` in your IDE or editor.

**Description:**
Translates a key using custom languagePath syntax for ContentBlocks.

**Snippet Code:**

```html
<f:translate
    key="{cb:languagePath(name: 'vendor/name')}:key"
    extensionName="my_ext"
    arguments="{
        0: 'argument1',
        1: 'argument2'
    }"
    default="Default translation"
/>
```

---

### Translate Inline ViewHelper (ContentBlocks)

**Trigger the Snippet:** Type `cbTranslateInline` in your IDE or editor.

**Description:**
Translates an inline key using custom languagePath syntax for ContentBlocks.

**Snippet Code:**

```html
{f:translate(key: '{cb:languagePath(name: 'vendor/name')}:key')}
```

---

### Uri Resource Inline ViewHelper (ContentBlocks)

**Trigger the Snippet:** Type `cbUriResourceInline` in your IDE or editor.

**Description:**
An inline version of the Uri Resource ViewHelper for ContentBlocks.

**Snippet Code:**

```html
{cb:uri.resource(path: 'foo.webp')}
```

---

### CSS Asset ViewHelper (ContentBlocks)

**Trigger the Snippet:** Type `cbAssetPathCss` in your IDE or editor.

**Description:**
Includes a CSS file in TYPO3 templates, identified by a unique identifier for ContentBlocks.

**Snippet Code:**

```html
<f:asset.css identifier="css" href="{cb:assetPath(name: 'vendor/name')}/frontend.css" />
```

---

### Script Asset ViewHelper (ContentBlocks)

**Trigger the Snippet:** Type `cbAssetPathScript` in your IDE or editor.

**Description:**
Includes a JavaScript file in TYPO3 templates, identified by a unique identifier for ContentBlocks.

**Snippet Code:**

```html
<f:asset.script identifier="js" href="{cb:assetPath(name: 'vendor/name')}/frontend.js" />
```
