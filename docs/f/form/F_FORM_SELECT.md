### Form Select Optgroup Tag

**Trigger the Snippet:** Type `fFormSelectOptgroup` in your IDE or editor to trigger this snippet.

**Description:**
Adds custom <optgroup> tags inside an <f:form.select>, supporting further child <f:form.select.option> tags. This is useful for grouping related options within a select dropdown in a form.

**Snippet Code:**

```html
<f:form.select.optgroup
    additionalAttributes="${1:array}"
    data="${2:array}"
    disabled="${3:false}"
>
    ${4}
</f:form.select.optgroup>
```

---

### Form Select Option Tag

**Trigger the Snippet:** Type `fFormSelectOption` in your IDE or editor to trigger this snippet.

**Description:**
Adds custom <option> tags inside an <f:form.select>. This allows you to define individual options within a select dropdown, with support for additional attributes and data.

**Snippet Code:**

```html
<f:form.select.option
    additionalAttributes="${1:array}"
    data="${2:array}"
    selected="${3}"
    value="${4}"
>
    ${5}
</f:form.select.option>
```
