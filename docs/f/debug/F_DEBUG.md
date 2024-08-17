### Backend Debug Render Tag

**Trigger the Snippet:** Type `fDebugRender` in your IDE or editor to trigger this snippet.

**Description:**
A debuggable version of `<f:render>` that wraps the output with HTML for inspection with the admin panel in the frontend. This tag is especially useful during development to visually inspect how partials and sections are rendered with provided arguments.

**Snippet Code:**

```html
<f:debug.render
    partial="${1:PartialName}"
    section="${2:SectionName}"
    arguments="${3:{_all}}"
    contentAs="${4:content}"
    debug="${5:true}"
    default="${6:DefaultValue}"
    optional="${7:false}"
>
</f:debug.render>
```
