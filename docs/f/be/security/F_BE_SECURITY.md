### Backend IfAuthenticated ViewHelper

**Trigger the Snippet:** Type `fBeSecurityIfAuthenticated` in your IDE or editor to trigger this snippet.

**Description:**
Renders the content inside this tag only if the backend user is authenticated.

**Snippet Code:**

```html
<f:be.security.ifAuthenticated>
    $1
</f:be.security.ifAuthenticated>
```

---

### Backend IfHasRole ViewHelper

**Trigger the Snippet:** Type `fBeSecurityIfHasRole` in your IDE or editor to trigger this snippet.

**Description:**
Renders the content inside this tag only if the backend user has the specified role.

**Snippet Code:**

```html
<f:be.security.ifHasRole role="$1">
    $2
</f:be.security.ifHasRole>
```
