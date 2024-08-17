### Format Bytes ViewHelper

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
>
    $5
</f:format.bytes>
```

---

### Format Bytes Inline ViewHelper

**Trigger the Snippet:** Type `fFormatBytesInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats an integer with a byte count into a human-readable form using the inline syntax.

**Snippet Code:**

```html
{${1:fileSize} -> f:format.bytes(decimalSeparator: '${2:.}', decimals: ${3:0}, thousandsSeparator: '${4:,}', units: '${5}')}
```

---

### Format Case ViewHelper

**Trigger the Snippet:** Type `fFormatCase` in your IDE or editor to trigger this snippet.

**Description:**
Modifies the case of an input string to upper- or lowercase or capitalization.

**Snippet Code:**

```html
<f:format.case mode="${1:upper}">
    $value
</f:format.case>
```

---

### Format Case Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCaseInline` in your IDE or editor to trigger this snippet.

**Description:**
Modifies the case of an input string to upper- or lowercase or capitalization using the inline syntax.

**Snippet Code:**

```html
{${1:someVariable} -> f:format.case(case: '${2:upper}')}
```

---

### Format Cdata ViewHelper

**Trigger the Snippet:** Type `fFormatCdata` in your IDE or editor to trigger this snippet.

**Description:**
Outputs an argument/value without any escaping and wraps it with CDATA tags.

**Snippet Code:**

```html
<f:format.cdata>
    $1
</f:format.cdata>
```

---

### Format Cdata Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCdataInline` in your IDE or editor to trigger this snippet.

**Description:**
Outputs an argument/value without any escaping and wraps it with CDATA tags using the inline syntax.

**Snippet Code:**

```html
{${1:string} -> f:format.cdata()}
```

---

### Format Crop ViewHelper

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

### Format Crop Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCropInline` in your IDE or editor to trigger this snippet.

**Description:**
Crops the text to a specified length, respecting HTML entities and word boundaries using the inline syntax.

**Snippet Code:**

```html
{${1:someLongText} -> f:format.crop(append: '${2:&hellip;}', maxCharacters: ${3:10}, respectHtml: ${4:true}, respectWordBoundaries: ${5:true})}
```

---

### Format Currency ViewHelper

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
    useDash="${7:false}"
>
    $8
</f:format.currency>
```

---

### Format Currency Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCurrencyInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats a given float to a currency representation using the inline syntax.

**Snippet Code:**

```html
{${1:someNumber} -> f:format.currency(thousandsSeparator: '${2:,}', currencySign: '${3:EUR}', decimalSeparator: '${4:.}', decimals: ${5:2}, prependCurrency: ${6:true}, separateCurrency: ${7:false}, useDash: ${8:false})}
```

---

### Format Date ViewHelper

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
    pattern="${5}"
>
    $6
</f:format.date>
```

---

### Format Date Inline ViewHelper

**Trigger the Snippet:** Type `fFormatDateInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats an object implementing \DateTimeInterface using the inline syntax.

**Snippet Code:**

```html
{f:format.date(base: '${1}', date: ${2:dateObject}, format: '${3:Y-m-d}', locale: '${4}', pattern: '${5}')}
```

---

### Format HTML ViewHelper

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
    table="${5}"
>
    $6
</f:format.html>
```

---

### Format HTML Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlInline` in your IDE or editor to trigger this snippet.

**Description:**
Renders a string by passing it to a TYPO3 parseFunc using the inline syntax.

**Snippet Code:**

```html
{${1:someText} -> f:format.html(parseFuncTSPath: '${2:lib.parseFunc}')}
```

---

### Format HtmlEntities ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlentities` in your IDE or editor to trigger this snippet.

**Description:**
Applies `htmlentities()` escaping to a value. This ViewHelper is useful for encoding special characters into HTML entities, enhancing security by preventing unintended HTML or script executions.

**Snippet Code:**

```html
<f:format.htmlentities
    doubleEncode="${1:true}"
    encoding="${2:UTF-8}"
    keepQuotes="${3:false}"
>
    $4
</f:format.htmlentities>
```

---

### Format HtmlEntities Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlentitiesInline` in your IDE or editor to trigger this snippet.

**Description:**
Applies htmlentities() escaping to a value using the inline syntax.

**Snippet Code:**

```html
{${1:text} -> f:format.htmlentities(encoding: '${2:ISO-8859-1}', doubleEncode: ${3:true}, keepQuotes: ${4:false})}
```

---

### Format HtmlEntitiesDecode ViewHelper

**Trigger the Snippet:** Type `htmlentitiesDecode` in your IDE or editor to trigger this snippet.

**Description:**
Applies `htmlentities()` escaping to a value. This ViewHelper is useful for encoding special characters into HTML entities, enhancing security by preventing unintended HTML or script executions.

**Snippet Code:**

```html
<f:format.htmlentitiesDecode
    encoding="${1:UTF-8}"
    keepQuotes="${2:false}"
>
    $3
</f:format.htmlentitiesDecode>
```

---

### Format HtmlEntitiesDecode Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlentitiesDecodeInline` in your IDE or editor to trigger this snippet.

**Description:**
Applies html_entity_decode() to a value using the inline syntax.

**Snippet Code:**

```html
{${1:text} -> f:format.htmlentitiesDecode(encoding: '${2:ISO-8859-1}', keepQuotes: ${3:false})}
```

---

### Format Htmlspecialchars ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlspecialchars` in your IDE or editor to trigger this snippet.

**Description:**
Applies PHP `htmlspecialchars()` escaping to a value. This ViewHelper helps prevent XSS attacks by converting special characters to their HTML entities.

**Snippet Code:**

```html
<f:format.htmlspecialchars
    doubleEncode="${1:true}"
    encoding="${2:UTF-8}"
    keepQuotes="${3:false}"
>
    $4
</f:format.htmlspecialchars>
```

---

### Format Htmlspecialchars Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlspecialcharsInline` in your IDE or editor to trigger this snippet.

**Description:**
Applies PHP htmlspecialchars() escaping to a value using the inline syntax.

**Snippet Code:**

```html
{${1:text} -> f:format.htmlspecialchars(encoding: '${2:ISO-8859-1}', doubleEncode: ${3:true}, keepQuotes: ${4:false})}
```

---

### Format Json ViewHelper

**Trigger the Snippet:** Type `fFormatJson` in your IDE or editor to trigger this snippet.

**Description:**
Wrapper for PHP's json_encode function. This ViewHelper is used to convert arrays or objects into JSON formatted strings.


**Snippet Code:**

```html
<f:format.json forceObject="${1:false}">
    $2
</f:format.json>
```

---

### Format Json Inline ViewHelper

**Trigger the Snippet:** Type `fFormatJsonInline` in your IDE or editor to trigger this snippet.

**Description:**
Converts arrays or objects into JSON formatted strings using the inline syntax.

**Snippet Code:**

```html
{f:format.json(forceObject: ${1:false}, value: ${2:{foo: 'bar', bar: 'baz'}})}
```

---

### Format Nl2br ViewHelper

**Trigger the Snippet:** Type `fFormatNl2br` in your IDE or editor to trigger this snippet.

**Description:**
Wrapper for PHP's nl2br function. This ViewHelper converts new lines (`\n`) in a string to `<br>` HTML tags.

**Snippet Code:**

```html
<f:format.nl2br>
    $1
</f:format.nl2br>
```

---

###Format Nl2br Inline ViewHelper

**Trigger the Snippet:** Type `fFormatNl2brInline` in your IDE or editor to trigger this snippet.

**Description:**
Converts new lines (\n) in a string to <br> HTML tags using the inline syntax.

**Snippet Code:**

```html
{${1:text_with_linebreaks} -> f:format.nl2br()}
```

---

### Format Number ViewHelper

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

### Format Number Inline ViewHelper

**Trigger the Snippet:** Type `fFormatNumberInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats a number with custom precision, decimal point, and grouped thousands using the inline syntax.

**Snippet Code:**

```html
{${1:number} -> f:format.number(decimals: ${2:1}, decimalSeparator: '${3:,}', thousandsSeparator: '${4:.}')}
```

---

### Format Padding ViewHelper

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
Formats a string using PHP's `str_pad` function, adding padding to the specified side.

**Snippet Code:**

```html
<f:format.padding
    padLength="${1:10}"
    padString="${2: }"
    padType="${3:right}"
>
    $4
</f:format.padding>
```

---

### Format Padding Inline ViewHelper

**Trigger the Snippet:** Type `fFormatPaddingInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats a string using PHP's str_pad function, adding padding to the specified side using the inline syntax.

**Snippet Code:**

```html
{${1:TYPO3} -> f:format.padding(padLength: ${2:10}, padString: '${3:-=}', padType: '${4:right}')}
```

---

### Format Printf ViewHelper

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
A ViewHelper for formatting values using the printf function, which allows for customized formatted output.

**Snippet Code:**

```html
<f:format.printf arguments="${1:array}">
    $3
</f:format.printf>
```

---

### Format Printf Inline ViewHelper

**Trigger the Snippet:** Type `fFormatPrintfInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats values using the printf function with inline syntax, allowing for customized formatted output.

**Snippet Code:**

```html
{${1:someText} -> f:format.printf(arguments: ${2:{1: 'TYPO3'}})}
```

---

### Format Raw ViewHelper

**Trigger the Snippet:** Type `fFormatRaw` in your IDE or editor to trigger this snippet.

**Description:**
Outputs a value without any escaping, preserving the raw data.

**Snippet Code:**

```html
<f:format.raw>
    ${1}
</f:format.raw>
```

---

### Format Raw Inline ViewHelper

**Trigger the Snippet:** Type `fFormatRawInline` in your IDE or editor to trigger this snippet.

**Description:**
Outputs a value without any escaping, preserving the raw data using the inline syntax.

**Snippet Code:**

```html
{${1:string} -> f:format.raw()}
```

---

### Format StripTags ViewHelper

**Trigger the Snippet:** Type `fFormatStripTags` in your IDE or editor to trigger this snippet.

**Description:**
Removes HTML and PHP tags from a string, optionally allowing certain tags.

**Snippet Code:**

```html
<f:format.stripTags allowedTags="${1}">
    $2
</f:format.stripTags>
```

---

### Format StripTags Inline ViewHelper

**Trigger the Snippet:** Type `fFormatStripTagsInline` in your IDE or editor to trigger this snippet.

**Description:**
Removes HTML and PHP tags from a string using the inline syntax, optionally allowing certain tags.

**Snippet Code:**

```html
{${1:text} -> f:format.stripTags(allowedTags: '${2}')}
```

---

### Format Trim ViewHelper

**Trigger the Snippet:** Type `fFormatTrim` in your IDE or editor to trigger this snippet.

**Description:**
Strips whitespace (or other specified characters) from the beginning and end of a string.

**Snippet Code:**

```html
<f:format.trim
    characters="${1}"
    side="${2:both}"
>
    $3
</f:format.trim>
```

---

### Format Trim Inline ViewHelper

**Trigger the Snippet:** Type `fFormatTrimInline` in your IDE or editor to trigger this snippet.

**Description:**
Strips whitespace (or other specified characters) from the beginning and end of a string using the inline syntax.

**Snippet Code:**

```html
{${1:yourString} -> f:format.trim(side: '${2:right}', characters: '${3}')}
```

---

### Format Urlencode ViewHelper

**Trigger the Snippet:** Type `fFormatUrlencode` in your IDE or editor to trigger this snippet.

**Description:**
Encodes a string using rawurlencode according to RFC 3986, making it safe to use in URLs.

**Snippet Code:**

```html
<f:format.urlencode>
    ${1}
</f:format.urlencode>
```

---

### Format Urlencode Inline ViewHelper

**Trigger the Snippet:** Type `fFormatUrlencodeInline` in your IDE or editor to trigger this snippet.

**Description:**
Encodes a string using rawurlencode according to RFC 3986, making it safe to use in URLs using the inline syntax.

**Snippet Code:**

```html
{${1:text} -> f:format.urlencode()}
```
