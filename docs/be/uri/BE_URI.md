### Edit Record URI ViewHelper

**Trigger the Snippet:** Type `beUriEditRecord` in your IDE or editor to trigger this snippet.

**Description:**
Generates a URI for editing a specific record. The URI includes parameters for the record UID, target table, and optional fields to edit. You can also specify a return URL to redirect after editing.

**Snippet Code:**

```html
<be:uri.editRecord
    uid="${1:42}"
    table="${2:a_table}"
    returnUrl="${3:foo/bar}"
    fields="${4:title,subtitle}"
/>
```

---

### Create New Record URI ViewHelper

**Trigger the Snippet:** Type `beUriNewRecord` in your IDE or editor to trigger this snippet.

**Description:**
Generates a URI for creating a new record. The URI includes parameters for the target table, page ID (pid), and optional UID for sorting. You can also set default values for fields and specify a return URL to redirect after creating the record.

**Snippet Code:**

```html
<be:uri.newRecord
    table="${1:a_table}"
    returnUrl="${2:foo/bar}"
    pid="${3:17}"
    uid="${4:-17}"
    defaultValues="${5:{a_table: {a_field: 'value'}}}"
/>
```
