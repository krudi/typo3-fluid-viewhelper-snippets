### Form Button Tag

**Trigger the Snippet:** Type `fFormButton` in your IDE or editor to trigger this snippet.

**Description:**
Creates a button, such as a reset or submit button, in a form.

**Snippet Code:**

```html
<f:form.button
    type="${1:reset}"
    name="${2:buttonName}"
>
    ${3:Button Label}
</f:form.button>
```

---

### Form Checkbox Basic Tag

**Trigger the Snippet:** Type `fFormCheckboxBasic` in your IDE or editor to trigger this snippet.

**Description:**
Creates a basic checkbox input element.

**Snippet Code:**

```html
<f:form.checkbox
    name="${1:myCheckBox}"
    value="${2:someValue}"
/>
```

---

### Form Checkbox Preselected Tag

**Trigger the Snippet:** Type `fFormCheckboxPreselected` in your IDE or editor to trigger this snippet.

**Description:**
Creates a checkbox input element with a preselected value.

**Snippet Code:**

```html
<f:form.checkbox
    name="${1:myCheckBox}"
    value="${2:someValue}"
    checked="${3:{object.value} == 5}"
/>
```

---

### Form Checkbox Bound Tag

**Trigger the Snippet:** Type `fFormCheckboxBound` in your IDE or editor to trigger this snippet.

**Description:**
Creates a checkbox input element bound to a property, with multiple selections.

**Snippet Code:**

```html
<f:form.checkbox
    property="${1:interests}"
    value="${2:TYPO3}"
    multiple="${3:1}"
/>
```

---

### Form Country Select Tag

**Trigger the Snippet:** Type `fFormCountrySelect` in your IDE or editor to trigger this snippet.

**Description:**
Renders a select tag with all available countries as options.

**Snippet Code:**

```html
<f:form.countrySelect
    name="${1:country}"
    value="${2:{defaultCountry}}"
>
```

---

### Form Hidden Tag

**Trigger the Snippet:** Type `fFormHidden` in your IDE or editor to trigger this snippet.

**Description:**
Renders a hidden input field.

**Snippet Code:**

```html
<f:form.hidden
    name="${1:myHiddenValue}"
    value="${2:42}"
/>
```

---

### Form Password Tag

**Trigger the Snippet:** Type `fFormPassword` in your IDE or editor to trigger this snippet.

**Description:**
Creates a password input field.

**Snippet Code:**

```html
<f:form.password
    name="${1:myPassword}"
/>
```

---

### Form Radio Basic Tag

**Trigger the Snippet:** Type `fFormRadioBasic` in your IDE or editor to trigger this snippet.

**Description:**
Creates a password input field.

**Snippet Code:**

```html
<f:form.radio
    name="${1:myRadioButton}"
    value="${2:someValue}"
/>
```

---

### Form Radio Bound Tag

**Trigger the Snippet:** Type `fFormRadioBound` in your IDE or editor to trigger this snippet.

**Description:**
Creates a radio button input element bound to a property.

**Snippet Code:**

```html
<f:form.radio
    property="${1:newsletter}"
    value="${2:1}"
/>
```

---

### Form Radio Multiple Tag

**Trigger the Snippet:** Type `fFormSelectBasic` in your IDE or editor to trigger this snippet.

**Description:**
Creates a basic select dropdown list.

**Snippet Code:**

```html
<f:form.select
    name="${1:paymentOptions}"
    options="${2:{payPal: 'PayPal International Services', visa: 'VISA Card'}}"
/>
```

---

### Form Select Preselected Tag

**Trigger the Snippet:** Type `fFormSelectPreselected` in your IDE or editor to trigger this snippet.

**Description:**
Creates a select dropdown list with a preselected option.

**Snippet Code:**

```html
<f:form.select
    name="${1:paymentOptions}"
    options="${2:{payPal: 'PayPal International Services', visa: 'VISA Card'}}"
    value="${3:visa}"
/>
```

---

### Form Select Grouped Tag

**Trigger the Snippet:** Type `fFormSelectGrouped` in your IDE or editor to trigger this snippet.

**Description:**
Creates a select dropdown list with grouped options.

**Snippet Code:**

```html
<f:form.select
    name="${1:myproperty}"
>
    <f:form.select.option value="1">Option one</f:form.select.option>
    <f:form.select.option value="2">Option two</f:form.select.option>
    <f:form.select.optgroup label="Group 1">
        <f:form.select.option value="3">Grouped option one</f:form.select.option>
        <f:form.select.option value="4">Grouped option two</f:form.select.option>
    </f:form.select.optgroup>
</f:form.select>
```

---

### Form Submit Tag

**Trigger the Snippet:** Type `fFormSubmit` in your IDE or editor to trigger this snippet.

**Description:**
Creates a submit button.

**Snippet Code:**

```html
<f:form.submit
    name="${1:mySubmit}"
    value="${2:Send Mail}"
>
    ${3:<button>dummy button</button>}
</f:form.submit>
```

---

### Form Textarea Tag

**Trigger the Snippet:** Type `fFormTextarea` in your IDE or editor to trigger this snippet.

**Description:**
Creates a textarea field.

**Snippet Code:**

```html
<f:form.textarea
    name="${1:myTextArea}"
    value="${2:This is shown inside the textarea}"
/>
```

---

### Form Textfield Tag

**Trigger the Snippet:** Type `fFormTextfield` in your IDE or editor to trigger this snippet.

**Description:**
Creates a text field input element.

**Snippet Code:**

```html
<f:form.textfield
    name="${1:myTextBox}"
    value="${2:default value}"
/>
```

---

### Form Upload Tag

**Trigger the Snippet:** Type `fFormUpload` in your IDE or editor to trigger this snippet.

**Description:**
Generates an input file element.

**Snippet Code:**

```html
<f:form.upload
    name="${1:file}"
/>
```

---

### Form ValidationResults Tag

**Trigger the Snippet:** Type `fFormValidationResults` in your IDE or editor to trigger this snippet.

**Description:**
Outputs validation results.

**Snippet Code:**

```html
<f:form.validationResults
    for="${1}"
    as="${2:'validationResults'}"
>
    ${3}
</f:form.validationResults>
```
