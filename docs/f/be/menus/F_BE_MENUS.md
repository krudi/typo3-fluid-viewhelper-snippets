### Backend ActionMenu ViewHelper

**Trigger the Snippet:** Type `fBeMenusActionMenu` in your IDE or editor to trigger this snippet.

**Description:**
Renders a select box to switch between multiple actions and controllers, similar to TYPO3's funcMenu.

**Snippet Code:**

```html
<f:be.menus.actionMenu
    additionalAttributes="${1:array}"
    aria="${2:array}"
    data="${3:array}"
    defaultController="${4}"
>
    $5
</f:be.menus.actionMenu>
```

---

### Backend ActionMenuItem ViewHelper

**Trigger the Snippet:** Type `fBeMenusActionMenuItem` in your IDE or editor to trigger this snippet.

**Description:**
Adds an item to an action menu in the backend with specified label, controller, and action.

**Snippet Code:**

```html
<f:be.menus.actionMenuItem
    label="$1"
    controller="$2"
    action="$3"
    additionalAttributes="${4:array}"
    arguments="${5:array}"
    aria="${6:array}"
    data="${7:array}"
/>
```

---

### Backend ActionMenuItemGroup ViewHelper

**Trigger the Snippet:** Type `fBeMenusActionMenuItemGroup` in your IDE or editor to trigger this snippet.

**Description:**
Groups options of an action menu.

**Snippet Code:**

```html
<f:be.menus.actionMenuItemGroup
    label="$1"
    additionalAttributes="${2:array}"
    aria="${3:array}"
    data="${4:array}"
>
    $5
</f:be.menus.actionMenuItemGroup>
```
