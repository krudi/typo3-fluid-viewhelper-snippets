### Backend ActionMenu ViewHelper

**Trigger the Snippet:** Type `fBeMenusActionMenu` in your IDE or editor to trigger this snippet.

**Description:**
Renders a select box to switch between multiple actions and controllers, similar to TYPO3's funcMenu.

**Snippet Code:**

```html
<f:be.menus.actionMenu
    additionalAttributes="{}"
    aria="{}"
    data="{}"
    defaultController="DefaultController"
>
    Menu items go here
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
    label="Item Label"
    controller="DefaultController"
    action="index"
    additionalAttributes="{}"
    arguments="{}"
    aria="{}"
    data="{}"
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
    label="Group Label"
    additionalAttributes="{}"
    aria="{}"
    data="{}"
>
    Grouped menu items go here
</f:be.menus.actionMenuItemGroup>
```
