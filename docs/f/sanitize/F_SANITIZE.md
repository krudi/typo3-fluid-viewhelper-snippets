### Sanitize HTML Tag

**Trigger the Snippet:** Type `fSanitizeHtml` in your IDE or editor.

**Description:**
A ViewHelper that passes the given content through TYPO3's html-sanitizer to mitigate potential cross-site scripting (XSS) occurrences. This is particularly useful for ensuring that any HTML content rendered in your templates is safe and sanitized according to the specified build configuration.

**Snippet Code:**

```html
<f:sanitize.html
    build="${1:default}">
    ${2}
</f:sanitize.html>
```
