### Date Picker Form ViewHelper

**Trigger the Snippet:** Type `formDatePicker` in your IDE or editor to trigger this snippet.

**Description:**
Displays a jQuery date picker for selecting dates. Requires jQuery UI to be included on the page. Customize the date format, initial date, and whether to enable the date picker. Supports additional attributes and custom data- attributes.

**Snippet Code:**

```html
<formvh:form.datePicker
    name="${1:dateField}"
    dateFormat="${2:Y-m-d}"
    enableDatePicker="${3:true}"
    initialDate="${4:2024-08-08}"
/>
```

---

### Time Picker Form ViewHelper

**Trigger the Snippet:** Type `formTimePicker` in your IDE or editor to trigger this snippet.

**Description:**
Displays a time picker with select boxes for hour and minute selection. Customize the time type (hour or minute), initial time, and additional attributes. Supports custom data- attributes and error handling.

**Snippet Code:**

```html
<formvh:form.timePicker
    name="${1:timeField}"
    timeType="${2:hour}"
    initialDate="${3:12:00}"
/>
```

---

### Uploaded Resource Form ViewHelper

**Trigger the Snippet:** Type `formUploadedResource` in your IDE or editor to trigger this snippet.

**Description:**
Handles uploaded files and displays previously uploaded images if the form is redisplayed due to validation errors. Customize the accepted file types, additional attributes, and error handling. Supports custom data- attributes.

**Snippet Code:**

```html
<formvh:form.uploadedResource
    name="${1:fileField}"
    accept="${2:['image/jpeg', 'image/png']}"
/>
```
