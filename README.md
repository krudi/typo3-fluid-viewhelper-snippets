# typo3-fluid-viewhelper-snippets

TYPO3 Fluid ViewHelper snippets plus TypoScript and TSConfig syntax highlighting for [Visual Studio Code](https://code.visualstudio.com).

## Source of snippets

All snippets included in this extension are created and adjusted based on the [TYPO3 ViewHelper Reference](https://docs.typo3.org/other/typo3/view-helper-reference/main/en-us/). These snippets are designed to make coding easier and are still being developed. Continual additions and improvements are made to cover more needs and stay up-to-date with the latest TYPO3 features.

## What's inside

- `f:*` Fluid ViewHelpers for assets, formatting, links, security, and more
- `be:*` backend helpers such as module links, thumbnails, and user avatars
- `core:*` core utilities including context helpers and various PSR-14 events
- `formvh:*` forms (translation, render section, errors, and dynamic fields)
- `cb:*` Content Blocks utilities like asset paths and translations

## Quick examples

### fAssetCss (trigger: `fAssetCss`)

```html
<f:asset.css identifier="site-css" src="EXT:my_ext/Resources/Public/Css/main.css" />
```

### fFormatDateInline (trigger: `fFormatDateInline`)

```html
{f:format.date(date: event.startDate, format: 'Y-m-d H:i')}
```

### fFormSelectGrouped (trigger: `fFormSelectGrouped`)

```html
<f:form.select name="options">
    <f:form.select.option value="1">Option one</f:form.select.option>
    <f:form.select.optgroup label="Group 1">
        <f:form.select.option value="2">Grouped option</f:form.select.option>
    </f:form.select.optgroup>
</f:form.select>
```

### cbTranslateInline (trigger: `cbTranslateInline`)

```html
{f:translate(key: "{cb:languagePath(name: 'vendor/name')}:title")}
```

### fFormatBytes (trigger: `fFormatBytes`)

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

### fPageHeaderData (trigger: `fPageHeaderData`)

```html
<f:page.headerData>
    <link rel="preconnect" href="https://cdn.example.com">
    <link rel="dns-prefetch" href="//cdn.example.com">
</f:page.headerData>
```

### fPageMeta (trigger: `fPageMeta`)

```html
<f:page.meta
    property="og:image"
    subProperties="{width: 1200, height: 630, alt: 'Article image'}"
>
    {item.image.url}
</f:page.meta>
```

## Syntax Support

This extension also provides syntax support for [TypoScript](https://docs.typo3.org/m/typo3/reference-typoscript/main/en-us/Index.html) and [TSConfig](https://docs.typo3.org/m/typo3/reference-tsconfig/main/en-us/Index.html#start).

## Developing and testing locally

- Install dependencies: `npm install`.
- Open the repo in VS Code and start an Extension Development Host: press `F5` (or run “Debug: Start Debugging”).
- In the new window, open `samples/sample.typoscript` or `samples/sample.tsconfig` to verify syntax highlighting and snippet triggers.
- To test a packaged build, run `vsce package` (after `npm install -g @vscode/vsce`), then in VS Code choose “Extensions” → “...” → “Install from VSIX...” and select the generated `.vsix`.

## Issue

Have you found a bug in this project or have a suggestion for a new feature? Create a new ticket for the bug or feature, which can be found on the [GitHub](https://github.com/krudi/typo3-fluid-viewhelper-snippets/issues) page.
