### Transform HTML ViewHelper

**Trigger the Snippet:** Type `fTransformHtml` in your IDE or editor.

**Description:**
This ViewHelper transforms HTML and substitutes internal link scheme aspects. It allows you to manipulate specific elements within your HTML content based on the provided CSS selector and handle failures according to the specified onFailure strategy.

**Snippet Code:**

```html
<f:transform.html
    onFailure="removeEnclosure"
    selector="a.href"
>
    <a href="t3://page?uid=1" class="home">Home</a>
</f:transform.html>
```

---

### Transform HTML ViewHelper

**Trigger the Snippet:** Type `fTransformHtmlInline` in your IDE or editor.

**Description:**
Inline version of the <f:transform.html> ViewHelper for transforming HTML.

**Snippet Code:**

```html
{content -> f:transform.html(selector: 'a.href', onFailure: 'removeEnclosure')}
```
