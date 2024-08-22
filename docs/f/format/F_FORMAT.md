### Format Bytes ViewHelper

**Trigger the Snippet:** Type `fFormatBytes` in your IDE or editor to trigger this snippet.

**Description:**
Formats an integer with a byte count into a human-readable form.

**Snippet Code:**

```html
<f:format.bytes
    decimalSeparator="."
    decimals="2"
    thousandsSeparator=","
    units="['B', 'KB', 'MB', 'GB', 'TB']"
>
    1048576
</f:format.bytes>
```

---

### Format Bytes Inline ViewHelper

**Trigger the Snippet:** Type `fFormatBytesInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats an integer with a byte count into a human-readable form using the inline syntax.

**Snippet Code:**

```html
{fileSize -> f:format.bytes(decimalSeparator: '.', decimals: 2, thousandsSeparator: ',', units: ['B', 'KB', 'MB', 'GB', 'TB'])}
```

---

### Format Case ViewHelper

**Trigger the Snippet:** Type `fFormatCase` in your IDE or editor to trigger this snippet.

**Description:**
Modifies the case of an input string to upper- or lowercase or capitalization.

**Snippet Code:**

```html
<f:format.case mode="upper">
    some text
</f:format.case>
```

---

### Format Case Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCaseInline` in your IDE or editor to trigger this snippet.

**Description:**
Modifies the case of an input string to upper- or lowercase or capitalization using the inline syntax.

**Snippet Code:**

```html
{someVariable -> f:format.case(mode: 'upper')}
```

---

### Format Cdata ViewHelper

**Trigger the Snippet:** Type `fFormatCdata` in your IDE or editor to trigger this snippet.

**Description:**
Outputs an argument/value without any escaping and wraps it with CDATA tags.

**Snippet Code:**

```html
<f:format.cdata>
    some content
</f:format.cdata>
```

---

### Format Cdata Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCdataInline` in your IDE or editor to trigger this snippet.

**Description:**
Outputs an argument/value without any escaping and wraps it with CDATA tags using the inline syntax.

**Snippet Code:**

```html
{string -> f:format.cdata()}
```

---

### Format Crop ViewHelper

**Trigger the Snippet:** Type `fFormatCrop` in your IDE or editor to trigger this snippet.

**Description:**
Crops the text between its opening and closing tags to a specified length, respecting HTML entities and word boundaries.

**Snippet Code:**

```html
<f:format.crop
    append="&hellip;"
    maxCharacters="100"
    respectHtml="true"
    respectWordBoundaries="true"
>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</f:format.crop>
```

---

### Format Crop Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCropInline` in your IDE or editor to trigger this snippet.

**Description:**
Crops the text to a specified length, respecting HTML entities and word boundaries using the inline syntax.

**Snippet Code:**

```html
{someLongText -> f:format.crop(append: '&hellip;', maxCharacters: 100, respectHtml: true, respectWordBoundaries: true)}
```

---

### Format Currency ViewHelper

**Trigger the Snippet:** Type `fFormatCurrency` in your IDE or editor to trigger this snippet.

**Description:**
Formats a given float to a currency representation. This ViewHelper is useful for displaying monetary values in the desired currency format.

**Snippet Code:**

```html
<f:format.currency
    currencySign="$"
    decimalSeparator="."
    decimals="2"
    prependCurrency="true"
    separateCurrency="false"
    thousandsSeparator=","
    useDash="false"
>
    1234.56
</f:format.currency>
```

---

### Format Currency Inline ViewHelper

**Trigger the Snippet:** Type `fFormatCurrencyInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats a given float to a currency representation using the inline syntax.

**Snippet Code:**

```html
{someNumber -> f:format.currency(thousandsSeparator: ',', currencySign: 'USD', decimalSeparator: '.', decimals: 2, prependCurrency: true, separateCurrency: false, useDash: false)}
```

---

### Format Date ViewHelper

**Trigger the Snippet:** Type `fFormatDate` in your IDE or editor to trigger this snippet.

**Description:**
Formats an object implementing `\DateTimeInterface`. This ViewHelper is especially useful for displaying dates in various formats according to local preferences.

**Snippet Code:**

```html
<f:format.date
    base="now"
    date=""
    format="Y-m-d"
    locale=""
    pattern=""
>
</f:format.date>
```

---

### Format Date Inline ViewHelper

**Trigger the Snippet:** Type `fFormatDateInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats an object implementing \DateTimeInterface using the inline syntax.

**Snippet Code:**

```html
{f:format.date(base: 'now', date: dateObject, format: 'Y-m-d', locale: '', pattern: '')}
```

---

### Format HTML ViewHelper

**Trigger the Snippet:** Type `fFormatHtml` in your IDE or editor to trigger this snippet.

**Description:**
Renders a string by passing it to a TYPO3 parseFunc, which allows for complex parsing rules defined in TypoScript. This is particularly useful for rendering rich text or formatted content that involves TypoScript configurations.

**Snippet Code:**

```html
<f:format.html
    current="someText"
    currentValueKey=""
    data=""
    parseFuncTSPath="lib.parseFunc_RTE"
    table="tt_content"
>
</f:format.html>
```

---

### Format HTML Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlInline` in your IDE or editor to trigger this snippet.

**Description:**
Renders a string by passing it to a TYPO3 parseFunc using the inline syntax.

**Snippet Code:**

```html
{someText -> f:format.html(parseFuncTSPath: 'lib.parseFunc_RTE')}
```

---

### Format HtmlEntities ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlentities` in your IDE or editor to trigger this snippet.

**Description:**
Applies `htmlentities()` escaping to a value. This ViewHelper is useful for encoding special characters into HTML entities, enhancing security by preventing unintended HTML or script executions.

**Snippet Code:**

```html
<f:format.htmlentities
    doubleEncode="true"
    encoding="UTF-8"
    keepQuotes="false"
>
    some <b>HTML</b> content
</f:format.htmlentities>
```

---

### Format HtmlEntities Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlentitiesInline` in your IDE or editor to trigger this snippet.

**Description:**
Applies htmlentities() escaping to a value using the inline syntax.

**Snippet Code:**

```html
{text -> f:format.htmlentities(encoding: 'UTF-8', doubleEncode: true, keepQuotes: false)}
```

---

### Format HtmlEntitiesDecode ViewHelper

**Trigger the Snippet:** Type `htmlentitiesDecode` in your IDE or editor to trigger this snippet.

**Description:**
Applies `htmlentities()` escaping to a value. This ViewHelper is useful for encoding special characters into HTML entities, enhancing security by preventing unintended HTML or script executions.

**Snippet Code:**

```html
<f:format.htmlentitiesDecode
    encoding="UTF-8"
    keepQuotes="false"
>
    some &lt;b&gt;HTML&lt;/b&gt; content
</f:format.htmlentitiesDecode>
```

---

### Format HtmlEntitiesDecode Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlentitiesDecodeInline` in your IDE or editor to trigger this snippet.

**Description:**
Applies html_entity_decode() to a value using the inline syntax.

**Snippet Code:**

```html
{text -> f:format.htmlentitiesDecode(encoding: 'UTF-8', keepQuotes: false)}
```

---

### Format Htmlspecialchars ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlspecialchars` in your IDE or editor to trigger this snippet.

**Description:**
Applies PHP `htmlspecialchars()` escaping to a value. This ViewHelper helps prevent XSS attacks by converting special characters to their HTML entities.

**Snippet Code:**

```html
<f:format.htmlspecialchars
    doubleEncode="true"
    encoding="UTF-8"
    keepQuotes="false"
>
    some <b>HTML</b> content
</f:format.htmlspecialchars>
```

---

### Format Htmlspecialchars Inline ViewHelper

**Trigger the Snippet:** Type `fFormatHtmlspecialcharsInline` in your IDE or editor to trigger this snippet.

**Description:**
Applies PHP htmlspecialchars() escaping to a value using the inline syntax.

**Snippet Code:**

```html
{text -> f:format.htmlspecialchars(encoding: 'UTF-8', doubleEncode: true, keepQuotes: false)}
```

---

### Format Json ViewHelper

**Trigger the Snippet:** Type `fFormatJson` in your IDE or editor to trigger this snippet.

**Description:**
Wrapper for PHP's json_encode function. This ViewHelper is used to convert arrays or objects into JSON formatted strings.


**Snippet Code:**

```html
<f:format.json forceObject="false">
    {foo: 'bar', bar: 'baz'}
</f:format.json>
```

---

### Format Json Inline ViewHelper

**Trigger the Snippet:** Type `fFormatJsonInline` in your IDE or editor to trigger this snippet.

**Description:**
Converts arrays or objects into JSON formatted strings using the inline syntax.

**Snippet Code:**

```html
{text -> f:format.htmlspecialchars(encoding: 'UTF-8', doubleEncode: true, keepQuotes: false)}
```

---

### Format Nl2br ViewHelper

**Trigger the Snippet:** Type `fFormatNl2br` in your IDE or editor to trigger this snippet.

**Description:**
Wrapper for PHP's nl2br function. This ViewHelper converts new lines (`\n`) in a string to `<br>` HTML tags.

**Snippet Code:**

```html
<f:format.nl2br>
    Line one\nLine two
</f:format.nl2br>
```

---

###Format Nl2br Inline ViewHelper

**Trigger the Snippet:** Type `fFormatNl2brInline` in your IDE or editor to trigger this snippet.

**Description:**
Converts new lines (\n) in a string to <br> HTML tags using the inline syntax.

**Snippet Code:**

```html
{text_with_linebreaks -> f:format.nl2br()}
```

---

### Format Number ViewHelper

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
Formats a number with custom precision, decimal point, and grouped thousands. Useful for displaying numerical data in a more readable format.
**Snippet Code:**

```html
<f:format.number
    decimalSeparator="."
    decimals="2"
    thousandsSeparator=","
>
    1234567.89
</f:format.number>
```

---

### Format Number Inline ViewHelper

**Trigger the Snippet:** Type `fFormatNumberInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats a number with custom precision, decimal point, and grouped thousands using the inline syntax.

**Snippet Code:**

```html
{number -> f:format.number(decimals: 2, decimalSeparator: '.', thousandsSeparator: ',')}
```

---

### Format Padding ViewHelper

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
Formats a string using PHP's `str_pad` function, adding padding to the specified side.

**Snippet Code:**

```html
<f:format.padding
    padLength="10"
    padString=" "
    padType="right"
>
    content
</f:format.padding>
```

---

### Format Padding Inline ViewHelper

**Trigger the Snippet:** Type `fFormatPaddingInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats a string using PHP's str_pad function, adding padding to the specified side using the inline syntax.

**Snippet Code:**

```html
{TYPO3 -> f:format.padding(padLength: 10, padString: '-=', padType: 'right')}
```

---

### Format Printf ViewHelper

**Trigger the Snippet:** Type `fFormatNumber` in your IDE or editor to trigger this snippet.

**Description:**
A ViewHelper for formatting values using the printf function, which allows for customized formatted output.

**Snippet Code:**

```html
<f:format.printf arguments="['TYPO3']">
    Hello, %s!
</f:format.printf>
```

---

### Format Printf Inline ViewHelper

**Trigger the Snippet:** Type `fFormatPrintfInline` in your IDE or editor to trigger this snippet.

**Description:**
Formats values using the printf function with inline syntax, allowing for customized formatted output.

**Snippet Code:**

```html
{someText -> f:format.printf(arguments: ['TYPO3'])}
```

---

### Format Raw ViewHelper

**Trigger the Snippet:** Type `fFormatRaw` in your IDE or editor to trigger this snippet.

**Description:**
Outputs a value without any escaping, preserving the raw data.

**Snippet Code:**

```html
<f:format.raw>
    some unescaped content
</f:format.raw>
```

---

### Format Raw Inline ViewHelper

**Trigger the Snippet:** Type `fFormatRawInline` in your IDE or editor to trigger this snippet.

**Description:**
Outputs a value without any escaping, preserving the raw data using the inline syntax.

**Snippet Code:**

```html
{string -> f:format.raw()}
```

---

### Format StripTags ViewHelper

**Trigger the Snippet:** Type `fFormatStripTags` in your IDE or editor to trigger this snippet.

**Description:**
Removes HTML and PHP tags from a string, optionally allowing certain tags.

**Snippet Code:**

```html
<f:format.stripTags allowedTags="<b><i>">
    some <b>HTML</b> content
</f:format.stripTags>
```

---

### Format StripTags Inline ViewHelper

**Trigger the Snippet:** Type `fFormatStripTagsInline` in your IDE or editor to trigger this snippet.

**Description:**
Removes HTML and PHP tags from a string using the inline syntax, optionally allowing certain tags.

**Snippet Code:**

```html
{text -> f:format.stripTags(allowedTags: '<b><i>')}
```

---

### Format Trim ViewHelper

**Trigger the Snippet:** Type `fFormatTrim` in your IDE or editor to trigger this snippet.

**Description:**
Strips whitespace (or other specified characters) from the beginning and end of a string.

**Snippet Code:**

```html
<f:format.trim
    characters=""
    side="both"
>
    some text
</f:format.trim>
```

---

### Format Trim Inline ViewHelper

**Trigger the Snippet:** Type `fFormatTrimInline` in your IDE or editor to trigger this snippet.

**Description:**
Strips whitespace (or other specified characters) from the beginning and end of a string using the inline syntax.

**Snippet Code:**

```html
{yourString -> f:format.trim(side: 'both', characters: ' ')}
```

---

### Format Urlencode ViewHelper

**Trigger the Snippet:** Type `fFormatUrlencode` in your IDE or editor to trigger this snippet.

**Description:**
Encodes a string using rawurlencode according to RFC 3986, making it safe to use in URLs.

**Snippet Code:**

```html
<f:format.urlencode>
    https://example.com/?q=some_value
</f:format.urlencode>
```

---

### Format Urlencode Inline ViewHelper

**Trigger the Snippet:** Type `fFormatUrlencodeInline` in your IDE or editor to trigger this snippet.

**Description:**
Encodes a string using rawurlencode according to RFC 3986, making it safe to use in URLs using the inline syntax.

**Snippet Code:**

```html
{text -> f:format.urlencode()}
```
