### Form Select Optgroup ViewHelper

**Trigger the Snippet:** Type `fFormSelectOptgroup` in your IDE or editor to trigger this snippet.

**Description:**
Adds custom <optgroup> tags inside an <f:form.select>, supporting further child <f:form.select.option> tags. This is useful for grouping related options within a select dropdown in a form.

**Snippet Code:**

```html
<f:form.select.optgroup
    additionalAttributes="{}"
    data="{}"
    disabled="false"
    label="Group Label"
>
    <f:form.select.option value="1">Option 1</f:form.select.option>
</f:form.select.optgroup>
```

---

### Form Select Option ViewHelper

**Trigger the Snippet:** Type `fFormSelectOption` in your IDE or editor to trigger this snippet.

**Description:**
Adds custom <option> tags inside an <f:form.select>. This allows you to define individual options within a select dropdown, with support for additional attributes and data.

**Snippet Code:**

```html
<f:form.select.option
    additionalAttributes="{}"
    data="{}"
    selected="false"
    value="optionValue"
>
    Option Label
</f:form.select.option>
```
