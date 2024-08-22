### User Avatar ViewHelper

**Trigger the Snippet:** Type `beAvatar` in your IDE or editor to trigger this snippet.

**Description:**
Renders the avatar for a specified backend user, including the `<img>` tag. You can specify the user ID, the size of the avatar, and whether to display a default icon if no custom avatar is set.

**Snippet Code:**

```html
<be:avatar
    backendUser="user.uid"
    size="32"
    showIcon="true"
/>
```

---

### Language Column ViewHelper

**Trigger the Snippet:** Type `beLanguageColumn` in your IDE or editor to trigger this snippet.

**Description:**
Accesses a specific column within a LanguageColumn object. Requires the column number and the LanguageColumn object as context to return the desired column.

**Snippet Code:**

```html
<be:languageColumn
    columnNumber="1"
    languageColumn="1"
/>
```

---

### Backend Module Link ViewHelper

**Trigger the Snippet:** Type `beModuleLink` in your IDE or editor to trigger this snippet.

**Description:**
Creates an internal link to a backend module. You can provide additional link arguments, include the current URL as a parameter, or use a query string for more complex linking.

**Snippet Code:**

```html
<be:moduleLink
    route="pages_new"
    arguments="{id:pageUid}"
/>
```

---

### Thumbnail Image ViewHelper

**Trigger the Snippet:** Type `beThumbnail` in your IDE or editor to trigger this snippet.

**Description:**
Generates an `<img>` tag for rendering thumbnails. The ViewHelper supports various image parameters including width, height, cropping, and context. You can also pass additional attributes and data for customization.

**Snippet Code:**

```html
<be:thumbnail
    image="file.resource"
    width="150"
    height="150"
    context="Image.Preview"
/>
```
