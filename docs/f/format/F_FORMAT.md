### Format Bytes Tag

**Trigger the Snippet:** Type `fFormatBytes` in your IDE or editor to trigger this snippet.

**Description:**
Formats an integer with a byte count into a human-readable form.

**Snippet Code:**

```html
<f:format.bytes
    decimalSeparator="${1:.}"
    decimals="${2:0}"
    thousandsSeparator="${3:,}"
    units="${4}"
    value="${5}">
    $6
</f:format.bytes>
```

---

### Format Case Tag

**Trigger the Snippet:** Type `fFormatCase` in your IDE or editor to trigger this snippet.

**Description:**
Modifies the case of an input string to upper- or lowercase or capitalization.

**Snippet Code:**

```html
<f:format.case
    mode="${1:upper}"
    value="${2}"
>
    $3
</f:format.case>
```

---

### Format Cdata Tag

**Trigger the Snippet:** Type `fFormatCdata` in your IDE or editor to trigger this snippet.

**Description:**
Outputs an argument/value without any escaping and wraps it with CDATA tags.

**Snippet Code:**

```html
<f:format.cdata
    value="${1}"
>
    $2
</f:format.cdata>
```

---

### Format Crop Tag

**Trigger the Snippet:** Type `fFormatCrop` in your IDE or editor to trigger this snippet.

**Description:**
Crops the text between its opening and closing tags to a specified length, respecting HTML entities and word boundaries.

**Snippet Code:**

```html
<f:format.crop
    append="${1:&hellip;}"
    maxCharacters="${2:10}"
    respectHtml="${3:true}"
    respectWordBoundaries="${4:true}"
>
    $5
</f:format.crop>
```

---

### Format Currency Tag

**Trigger the Snippet:** Type `fFormatCurrency` in your IDE or editor to trigger this snippet.

**Description:**
Formats a given float to a currency representation. This ViewHelper is useful for displaying monetary values in the desired currency format.

**Snippet Code:**

```html
<f:format.currency
    currencySign="${1:$}"
    decimalSeparator="${2:.}"
    decimals="${3:2}"
    prependCurrency="${4:true}"
    separateCurrency="${5:false}"
    thousandsSeparator="${6:,}"
    useDash="${7:false}">
    $8
</f:format.currency>
```

---

### Format Currency Tag

**Trigger the Snippet:** Type `fFormatDate` in your IDE or editor to trigger this snippet.

**Description:**
Formats an object implementing `\DateTimeInterface`. This ViewHelper is especially useful for displaying dates in various formats according to local preferences.

**Snippet Code:**

```html
<f:format.date
    base="${1}"
    date="${2}"
    format="${3:Y-m-d}"
    locale="${4}"
    pattern="${5}">
    $6
</f:format.date>
```

---

### Format HTML Tag

**Trigger the Snippet:** Type `fFormatHtml` in your IDE or editor to trigger this snippet.

**Description:**
Renders a string by passing it to a TYPO3 parseFunc, which allows for complex parsing rules defined in TypoScript. This is particularly useful for rendering rich text or formatted content that involves TypoScript configurations.

**Snippet Code:**

```html
<f:format.html
    current="${1}"
    currentValueKey="${2}"
    data="${3}"
    parseFuncTSPath="${4:lib.parseFunc_RTE}"
    table="${5}">
    $6
</f:format.html>
```

---

### Format HtmlEntities Tag

**Trigger the Snippet:** Type `fFormatHtmlentities` in your IDE or editor to trigger this snippet.

**Description:**
Applies `htmlentities()` escaping to a value. This ViewHelper is useful for encoding special characters into HTML entities, enhancing security by preventing unintended HTML or script executions.

**Snippet Code:**

```html
<f:format.htmlentities
    doubleEncode="${1:true}"
    encoding="${2:UTF-8}"
    keepQuotes="${3:false}"
    value="${4}">
    $5
</f:format.htmlentities>
```

---

### Format HtmlEntitiesDecode Tag

**Trigger the Snippet:** Type `htmlentitiesDecode` in your IDE or editor to trigger this snippet.

**Description:**
Applies `htmlentities()` escaping to a value. This ViewHelper is useful for encoding special characters into HTML entities, enhancing security by preventing unintended HTML or script executions.

**Snippet Code:**

```html
<f:format.htmlentitiesDecode
    encoding="${1:UTF-8}"
    keepQuotes="${2:false}"
    value="${3}">
    $4
</f:format.htmlentitiesDecode>
```

---

### Format Htmlspecialchars Tag

**Trigger the Snippet:** Type `fFormatHtmlspecialchars` in your IDE or editor to trigger this snippet.

**Description:**
Applies PHP `htmlspecialchars()` escaping to a value. This ViewHelper helps prevent XSS attacks by converting special characters to their HTML entities.

**Snippet Code:**

```html
<f:format.htmlspecialchars
    doubleEncode="${1:true}"
    encoding="${2:UTF-8}"
    keepQuotes="${3:false}"
    value="${4}"
>
    $5
</f:format.htmlspecialchars>
```

---

### Format Json Tag

**Trigger the Snippet:** Type `fFormatJson` in your IDE or editor to trigger this snippet.

**Description:**
Wrapper for PHP's json_encode function. This ViewHelper is used to convert arrays or objects into JSON formatted strings.


**Snippet Code:**

```html
<f:format.json
    forceObject="${1:false}"
    value="${2}"
>
    $3
</f:format.json>
```

---

### Format Nl2br Tag

**Trigger the Snippet:** Type `fFormatNl2br` in your IDE or editor to trigger this snippet.

**Description:**
Wrapper for PHP's nl2br function. This ViewHelper converts new lines (`\n`) in a string to `<br>` HTML tags.

**Snippet Code:**

```html
<f:format.nl2br
    value="${1}"
>
    $2
</f:format.nl2br>
```

---

### Format Number Tag

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
Formats a number with custom precision, decimal point, and grouped thousands. Useful for displaying numerical data in a more readable format.
**Snippet Code:**

```html
<f:format.number
    decimalSeparator="${1:.}"
    decimals="${2:2}"
    thousandsSeparator="${3:,}"
>
    $4
</f:format.number>

---

### Format Padding Tag

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
Formats a string using PHP's `str_pad` function, adding padding to the specified side.

**Snippet Code:**

```html
<f:format.padding
    padLength="${1:10}"
    padString="${2: }"
    padType="${3:right}"
    value="${4}"
>
    $5
</f:format.padding>
```

---

### Format Printf Tag

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
A ViewHelper for formatting values using the printf function, which allows for customized formatted output.

**Snippet Code:**

```html
<f:format.printf
    arguments="${1:array}"
    value="${2}"
>
    $3
</f:format.printf>
```

---

### Format Raw Tag

**Trigger the Snippet:** Type `fFormatRaw` in your IDE or editor to trigger this snippet.

**Description:**
Outputs a value without any escaping, preserving the raw data.

**Snippet Code:**

```html
<f:format.raw
    value="${1}"
>
    $2
</f:format.raw>
```

---

### Format StripTags Tag

**Trigger the Snippet:** Type `fFormatStripTags` in your IDE or editor to trigger this snippet.

**Description:**
Removes HTML and PHP tags from a string, optionally allowing certain tags.

**Snippet Code:**

```html
<f:format.stripTags
    allowedTags="${1}"
    value="${2}"
>
    $3
</f:format.stripTags>
```

---

### Format Trim Tag

**Trigger the Snippet:** Type `fFormatTrim` in your IDE or editor to trigger this snippet.

**Description:**
Strips whitespace (or other specified characters) from the beginning and end of a string.

**Snippet Code:**

```html
<f:format.trim
    characters="${1}"
    side="${2:both}"
    value="${3}"
>
    $4
</f:format.trim>
```

---

### Format Urlencode Tag

**Trigger the Snippet:** Type `fFormatUrlencode` in your IDE or editor to trigger this snippet.

**Description:**
Encodes a string using rawurlencode according to RFC 3986, making it safe to use in URLs.

**Snippet Code:**

```html
<f:format.urlencode
    value="${1}"
>
    $2
</f:format.urlencode>
```
