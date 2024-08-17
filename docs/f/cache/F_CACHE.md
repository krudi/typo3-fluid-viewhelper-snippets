### Backend Cache Disable ViewHelper

**Trigger the Snippet:** Type `fCacheDisable` in your IDE or editor to trigger this snippet.

**Description:**
Disables template compiling for the full template file to a PHP class.

**Snippet Code:**

```html
<f:cache.disable>
    $1
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
    $1
</f:cache.static>
```

---

### Backend Cache Static ViewHelper

**Trigger the Snippet:** Type `fCacheWarmup` in your IDE or editor to trigger this snippet.

**Description:**
Inserts variables that apply only during cache warmup and if no other variables are specified.

**Snippet Code:**

```html
<f:cache.warmup variables="${1:{foo: bar}}">
    $2
</f:cache.warmup>
```
