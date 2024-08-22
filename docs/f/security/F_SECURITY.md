### Security IfAuthenticated ViewHelper

**Trigger the Snippet:** Type `fSecurityIfAuthenticated` in your IDE or editor.

**Description:**
This ViewHelper implements an ifAuthenticated/else condition for frontend users. It allows you to display different content based on whether a frontend (FE) user is logged in or not.

**Snippet Code:**

```html
<f:security.ifAuthenticated>
  <f:then>
    You are logged in as a frontend user.
  </f:then>
  <f:else>
    Please log in to access this content.
  </f:else>
</f:security.ifAuthenticated>
```

---

### Security IfHasRole ViewHelper

**Trigger the Snippet:** Type `fSecurityIfHasRole` in your IDE or editor.

**Description:**
This ViewHelper implements an ifHasRole/else condition for frontend groups. It allows you to display different content based on whether a user has a specific role (e.g., Administrator).

**Snippet Code:**

```html
<f:security.ifHasRole role="Administrator">
  <f:then>
    Welcome, Administrator!
  </f:then>
  <f:else>
    You do not have the necessary permissions.
  </f:else>
</f:security.ifHasRole>
```

---

### Security Nonce ViewHelper

**Trigger the Snippet:** Type `fSecurityNonce` in your IDE or editor.

**Description:**
This ViewHelper resolves the nonce attribute from the global server request object, or from the PolicyProvider service as a fallback value. It is useful for adding security nonces to inline scripts to enhance Content Security Policy (CSP) compliance.

**Snippet Code:**

```html
<script nonce="{f:security.nonce()}">
  const inlineScript = 'This script is secured with a nonce.';
</script>
```
