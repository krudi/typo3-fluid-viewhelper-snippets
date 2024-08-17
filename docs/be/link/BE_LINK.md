### Edit Record Link ViewHelper

**Trigger the Snippet:** Type `beLinkEditRecord` in your IDE or editor to trigger this snippet.

**Description:**
Generates a link to edit a specific record identified by its UID and table. You can specify fields to edit and a return URL to redirect after closing the edit dialog.

**Snippet Code:**

```html
<be:link.editRecord
    uid="${1:42}"
    table="${2:a_table}"
    ${3:returnUrl="foo/bar"}
    ${4:fields=""}
/>

---

### New Record Link ViewHelper

**Trigger the Snippet:** Type `beLinkNewRecord` in your IDE or editor to trigger this snippet.

**Description:**
Generates a link to create a new record in a specified table. You can specify the page ID for placement, the UID for ordering, default field values, and a return URL to redirect after creating the record.

**Snippet Code:**

```html
<be:link.newRecord
    table="${1:a_table}"
    ${2:pid=""}
    ${3:uid="-17"}
    ${4:returnUrl="foo/bar"}
    ${5:defaultValues="{}"}
/>
```
