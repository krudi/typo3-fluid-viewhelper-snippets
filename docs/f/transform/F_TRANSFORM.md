### Transform HTML ViewHelper

**Trigger the Snippet:** Type `fTransformHtml` in your IDE or editor.

**Description:**
This ViewHelper transforms HTML and substitutes internal link scheme aspects. It allows you to manipulate specific elements within your HTML content based on the provided CSS selector and handle failures according to the specified onFailure strategy.

**Snippet Code:**

```html
<f:transform.html
    onFailure="${1:removeEnclosure}"
    selector="${2:a.href}"
>
    ${3}
</f:transform.html>
```
