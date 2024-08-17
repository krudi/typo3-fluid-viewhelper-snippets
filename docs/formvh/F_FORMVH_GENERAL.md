### Custom Form ViewHelper

**Trigger the Snippet:** Type `vhForm` in your IDE or editor to trigger this snippet.

**Description:**
Renders a form with custom configuration, including action URI, query parameters, and form method. Supports a wide range of attributes including action, controller, extension name, and more. Allows additional attributes, custom data attributes, and error handling.

**Snippet Code:**

```html
<formvh:form
    name="${1:formName}"
    action="${2:action}"
    method="${3:post}"
    controller="${4:controller}"
    extensionName="${5:extension}"
    format="${6:.html}"
/>
```

---

### Grid Column Class Auto Configuration ViewHelper

**Trigger the Snippet:** Type `vhGridColumnClassAutoConfiguration` in your IDE or editor to trigger this snippet.

**Description:**
Automatically configures grid column classes for a given renderable element. Requires a RootRenderableInterface instance to operate. Used to ensure consistent grid column styling in forms.

**Snippet Code:**

```html
<formvh:gridColumnClassAutoConfiguration
    element="${1:element}"
/>
```

---

### Render Form ViewHelper

**Trigger the Snippet:** Type `vhRender` in your IDE or editor to trigger this snippet.

**Description:**
Main entry point to render a form into a Fluid template. Requires a factory class that implements FormFactoryInterface. Supports custom factory configurations and prototypes.

**Snippet Code:**

```html
<formvh:render
    factoryClass="${1:YourCustomFactoryClass}"
    prototypeName="${2:yourPrototype}"
/>

---

### Render All Form Values ViewHelper

**Trigger the Snippet:** Type `vhRenderAllFormValues` in your IDE or editor to trigger this snippet.

**Description:**
Renders all values of a form. Outputs the values under the specified name in the template. Requires a RootRenderableInterface instance to provide the form values.

**Snippet Code:**

```html
<formvh:renderAllFormValues
    as="${1:formValue}"
    renderable="${2:renderableElement}"
/>
```

---

### Render Form Value ViewHelper

**Trigger the Snippet:** Type `vhRenderFormValue` in your IDE or editor to trigger this snippet.

**Description:**
Renders a single value of a form. Outputs the value under the specified name in the template. Requires a RenderableInterface instance to provide the form value.

**Snippet Code:**

```html
<formvh:renderFormValue
    as="${1:formValue}"
    renderable="${2:renderableElement}"
/>
```

---

### Render Renderable ViewHelper

**Trigger the Snippet:** Type `vhRenderRenderable` in your IDE or editor to trigger this snippet.

**Description:**
Renders a renderable element within a form. Requires a RenderableInterface instance and integrates with the TYPO3 CMS Form MVC View to return the rendered content.

**Snippet Code:**

```html
<formvh:renderRenderable
    renderable="${1:renderableElement}"
/>
```

---

### Translate Element Error ViewHelper

**Trigger the Snippet:** Type `vhTranslateElementError` in your IDE or editor to trigger this snippet.

**Description:**
Translates error messages for a form element. Requires both a Form Element and an Error object to perform the translation, making error messages localized for the user.

**Snippet Code:**

```html
<formvh:translateElementError
    element="${1:formElement}"
    error="${2:error}"
/>
```

---

### Translate Element Property ViewHelper

**Trigger the Snippet:** Type `vhTranslateElementProperty` in your IDE or editor to trigger this snippet.

**Description:**
Translates properties of a form element, allowing for localization of form fields and options. Requires a Form Element and the property to translate, along with optional rendering options.

**Snippet Code:**

```html
<formvh:translateElementProperty
    element="${1:formElement}"
    property="${2:property}"
    renderingOptionProperty="${3:renderingOption}"
/>
```
