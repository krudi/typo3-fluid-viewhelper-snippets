### Edit Record Link ViewHelper

**Trigger the Snippet:** Type `beLinkEditRecord` in your IDE or editor to trigger this snippet.

**Description:**
Generates a link to edit a specific record identified by its UID and table. You can specify fields to edit and a return URL to redirect after closing the edit dialog.

**Snippet Code:**

```html
<be:link.editRecord
    uid="42"
    table="tt_content"
    returnUrl="foo/bar"
    fields="title,subtitle"
/>
```

---

### New Record Link ViewHelper

**Trigger the Snippet:** Type `beLinkNewRecord` in your IDE or editor to trigger this snippet.

**Description:**
Generates a link to create a new record in a specified table. You can specify the page ID for placement, the UID for ordering, default field values, and a return URL to redirect after creating the record.

**Snippet Code:**

```html
<be:link.newRecord
    table="tt_content"
    pid="1"
    uid="-17"
    returnUrl="foo/bar"
    defaultValues="{tt_content: {header: 'New Header'}}"
/>
```
