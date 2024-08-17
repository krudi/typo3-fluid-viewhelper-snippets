### Security IfAuthenticated Tag

**Trigger the Snippet:** Type `fSecurityIfAuthenticated` in your IDE or editor.

**Description:**
This ViewHelper implements an ifAuthenticated/else condition for frontend users. It allows you to display different content based on whether a frontend (FE) user is logged in or not.

**Snippet Code:**

```html
<f:security.ifAuthenticated>
    <f:then>
        ${1:This is being shown whenever a FE user is logged in}
    </f:then>
    <f:else>
        ${2:This is being displayed if no FE user is logged in}
    </f:else>
</f:security.ifAuthenticated>
```

---

### Security IfHasRole Tag

**Trigger the Snippet:** Type `fSecurityIfHasRole` in your IDE or editor.

**Description:**
This ViewHelper implements an ifHasRole/else condition for frontend groups. It allows you to display different content based on whether a user has a specific role (e.g., Administrator).

**Snippet Code:**

```html
<f:security.ifHasRole role="${1:Administrator}">
    <f:then>
        ${2:This is being shown in case you have the role.}
    </f:then>
    <f:else>
        ${3:This is being displayed in case you do not have the role.}
    </f:else>
</f:security.ifHasRole>
```

---

### Security Nonce Tag

**Trigger the Snippet:** Type `fSecurityNonce` in your IDE or editor.

**Description:**
This ViewHelper resolves the nonce attribute from the global server request object, or from the PolicyProvider service as a fallback value. It is useful for adding security nonces to inline scripts to enhance Content Security Policy (CSP) compliance.

**Snippet Code:**

```html
<script nonce="{f:security.nonce()}">
    ${1:const inline = 'script';}
</script>
```
