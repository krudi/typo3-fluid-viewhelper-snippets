### Backend Cache Disable ViewHelper

**Trigger the Snippet:** Type `fCacheDisable` in your IDE or editor to trigger this snippet.

**Description:**
Disables template compiling for the full template file to a PHP class.

**Snippet Code:**

```html
<f:cache.disable>
    Cache is disabled for this block
</f:cache.disable>
```

---

### Backend Cache Static ViewHelper

**Trigger the Snippet:** Type `fCacheStatic` in your IDE or editor to trigger this snippet.

**Description:**
Forces the output of the enclosed template code to be compiled to a static string.

**Snippet Code:**

```html
<f:cache.static>
    This block will be statically cached
</f:cache.static>
```

---

### Backend Cache Static ViewHelper

**Trigger the Snippet:** Type `fCacheWarmup` in your IDE or editor to trigger this snippet.

**Description:**
Inserts variables that apply only during cache warmup and if no other variables are specified.

**Snippet Code:**

```html
<f:cache.warmup variables="{foo: 'bar'}">
    Content rendered during cache warmup
</f:cache.warmup>
```
