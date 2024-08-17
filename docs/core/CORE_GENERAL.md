### Normalized URL ViewHelper

**Trigger the Snippet:** Type `coreNormalizedUrl` in your IDE or editor to trigger this snippet.

**Description:**
Normalizes a path that uses EXT: syntax or an absolute URL to an absolute web path.

**Snippet Code:**

```html
<core:normalizedUrl pathOrUrl="${1:https://foo.bar/img.jpg}" />
```

---

### Icon for Resource ViewHelper

**Trigger the Snippet:** Type `coreIconForResource` in your IDE or editor to trigger this snippet.

**Description:**
Displays an icon for a FAL resource (file or folder).

**Snippet Code:**

```html
<core:iconForResource resource="{${1:file.resource}}" />
```

---

### Icon ViewHelper

**Trigger the Snippet:** Type `coreIcon` in your IDE or editor to trigger this snippet.

**Description:**
Displays an icon identified by an icon identifier.

**Snippet Code:**

```html
<core:icon
    title="${1:Open actions menu}"
    identifier="${2:actions-menu}"
    alternativeMarkupIdentifier="${3:inline}"
/>
```

---

### Icon for Record ViewHelper

**Trigger the Snippet:** Type `coreIconForRecord` in your IDE or editor to trigger this snippet.

**Description:**
Displays an icon for a specific record.

**Snippet Code:**

```html
<core:iconForRecord
    table="${1:tt_content}"
    row="{${2:record}}"
/>
```
