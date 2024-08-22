### Backend Debug Render ViewHelper

**Trigger the Snippet:** Type `fDebugRender` in your IDE or editor to trigger this snippet.

**Description:**
A debuggable version of `<f:render>` that wraps the output with HTML for inspection with the admin panel in the frontend. This tag is especially useful during development to visually inspect how partials and sections are rendered with provided arguments.

**Snippet Code:**

```html
<f:debug.render
    partial="PartialName"
    section="SectionName"
    arguments="{_all}"
    contentAs="content"
    debug="true"
    default="Default content"
    optional="false"
>
</f:debug.render>
```
