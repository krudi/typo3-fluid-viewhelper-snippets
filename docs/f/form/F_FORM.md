### Form Button ViewHelper

**Trigger the Snippet:** Type `fFormButton` in your IDE or editor to trigger this snippet.

**Description:**
Creates a button, such as a reset or submit button, in a form.

**Snippet Code:**

```html
<f:form.button
    type="submit"
    name="submitButton"
>
    Submit
</f:form.button>
```

---

### Form Checkbox Basic ViewHelper

**Trigger the Snippet:** Type `fFormCheckboxBasic` in your IDE or editor to trigger this snippet.

**Description:**
Creates a basic checkbox input element.

**Snippet Code:**

```html
<f:form.checkbox
    name="myCheckBox"
    value="1"
/>
```

---

### Form Checkbox Preselected ViewHelper

**Trigger the Snippet:** Type `fFormCheckboxPreselected` in your IDE or editor to trigger this snippet.

**Description:**
Creates a checkbox input element with a preselected value.

**Snippet Code:**

```html
<f:form.checkbox
    name="myCheckBox"
    value="1"
    checked="{object.value} == 1"
/>
```

---

### Form Checkbox Bound ViewHelper

**Trigger the Snippet:** Type `fFormCheckboxBound` in your IDE or editor to trigger this snippet.

**Description:**
Creates a checkbox input element bound to a property, with multiple selections.

**Snippet Code:**

```html
<f:form.checkbox
    property="interests"
    value="TYPO3"
    multiple="1"
/>
```

---

### Form Country Select ViewHelper

**Trigger the Snippet:** Type `fFormCountrySelect` in your IDE or editor to trigger this snippet.

**Description:**
Renders a select tag with all available countries as options.

**Snippet Code:**

```html
<f:form.countrySelect
    name="country"
    value="DE"
>
```

---

### Form Hidden ViewHelper

**Trigger the Snippet:** Type `fFormHidden` in your IDE or editor to trigger this snippet.

**Description:**
Renders a hidden input field.

**Snippet Code:**

```html
<f:form.hidden
    name="myHiddenValue"
    value="42"
/>
```

---

### Form Password ViewHelper

**Trigger the Snippet:** Type `fFormPassword` in your IDE or editor to trigger this snippet.

**Description:**
Creates a password input field.

**Snippet Code:**

```html
<f:form.password
    name="password"
    value=""
/>
```

---

### Form Radio Basic ViewHelper

**Trigger the Snippet:** Type `fFormRadioBasic` in your IDE or editor to trigger this snippet.

**Description:**
Creates a password input field.

**Snippet Code:**

```html
<f:form.radio
    name="myRadioButton"
    value="1"
/>
```

---

### Form Radio Bound ViewHelper

**Trigger the Snippet:** Type `fFormRadioBound` in your IDE or editor to trigger this snippet.

**Description:**
Creates a radio button input element bound to a property.

**Snippet Code:**

```html
<f:form.radio
    property="newsletter"
    value="1"
/>
```

---

### Form Radio Bound ViewHelper

**Trigger the Snippet:** Type `fFormRadioMultiple` in your IDE or editor to trigger this snippet.

**Description:**
Creates multiple radio button input elements.

**Snippet Code:**

```html
<f:form.radio
    name="myRadioButton"
    value="option1"
/>
<f:form.radio
    name="myRadioButton"
    value="option2"
/>
```

---

### Form Select Basic ViewHelper

**Trigger the Snippet:** Type `fFormSelectBasic` in your IDE or editor to trigger this snippet.

**Description:**
Creates a basic select dropdown list.

**Snippet Code:**

```html
<f:form.select
    name="paymentOptions"
    options="{'paypal': 'PayPal', 'visa': 'VISA'}"
/>
```

---

### Form Select Preselected ViewHelper

**Trigger the Snippet:** Type `fFormSelectPreselected` in your IDE or editor to trigger this snippet.

**Description:**
Creates a select dropdown list with a preselected option.

**Snippet Code:**

```html
<f:form.select
    name="paymentOptions"
    options="{'paypal': 'PayPal', 'visa': 'VISA'}"
    value="visa"
/>
```

---

### Form Select Grouped ViewHelper

**Trigger the Snippet:** Type `fFormSelectGrouped` in your IDE or editor to trigger this snippet.

**Description:**
Creates a select dropdown list with grouped options.

**Snippet Code:**

```html
<f:form.select
    name="options">
    <f:form.select.option value="1">Option one</f:form.select.option>
    <f:form.select.option value="2">Option two</f:form.select.option>
    <f:form.select.optgroup label="Group 1">
        <f:form.select.option value="3">Grouped option one</f:form.select.option>
        <f:form.select.option value="4">Grouped option two</f:form.select.option>
    </f:form.select.optgroup>
</f:form.select>
```

---

### Form Submit ViewHelper

**Trigger the Snippet:** Type `fFormSubmit` in your IDE or editor to trigger this snippet.

**Description:**
Creates a submit button.

**Snippet Code:**

```html
<f:form.submit
    name="mySubmit"
    value="Submit"
>
    Additional content
</f:form.submit>
```

---

### Form Textarea ViewHelper

**Trigger the Snippet:** Type `fFormTextarea` in your IDE or editor to trigger this snippet.

**Description:**
Creates a textarea field.

**Snippet Code:**

```html
<f:form.textarea
    name="myTextArea"
    value="Enter your text here"
/>
```

---

### Form Textfield ViewHelper

**Trigger the Snippet:** Type `fFormTextfield` in your IDE or editor to trigger this snippet.

**Description:**
Creates a text field input element.

**Snippet Code:**

```html
<f:form.textfield
    name="myTextBox"
    value="default value"
/>
```

---

### Form Upload ViewHelper

**Trigger the Snippet:** Type `fFormUpload` in your IDE or editor to trigger this snippet.

**Description:**
Generates an input file element.

**Snippet Code:**

```html
<f:form.upload
    name="fileUpload"
    value=""
/>
```

---

### Form ValidationResults ViewHelper

**Trigger the Snippet:** Type `fFormValidationResults` in your IDE or editor to trigger this snippet.

**Description:**
Outputs validation results.

**Snippet Code:**

```html
<f:form.validationResults
    for="object"
    as="validationResults"
>
    validation messages
</f:form.validationResults>
```
