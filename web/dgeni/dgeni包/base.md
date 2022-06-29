
## base

### 处理器

* `computeIdsProcessor` - Computes the `id` and `aliases` for documents using templates or helper functions, on a per docType basis.
* `computePathsProcessor` - Computes the `path` and `outputPath` for documents using templates or helper functions, on a per docType basis.
* `debugDumpProcessor` - dump the current state of the docs array to a file (disabled by default)
* `readFilesProcessor` - used to load up documents from files.  This processor can be configured to use a set of **file readers**. There are file readers in the `jsdoc` and `ngdoc` packages.
* `renderDocsProcessor` - render the documents into a property (`doc.renderedContent`) using a `templateEngine`, which must be provided separately - see `nunjucks` package.
* `unescapeCommentsProcessor` - unescape comment markers that would break the jsdoc comment style, e.g. `*/`
* `writeFilesProcessor` - write the docs that have an `outputPath` to disk

### 服务

* `aliasMap` - A map of ids/aliases to docs.  This is used for matching references to documents in links and relations such as modules and object members.
* `createDocMessage` - a helper for creating nice messages about documents (useful in logging and errors)
* `encodeDocBlock` - convert a block of code into HTML
* `templateFinder` - search folders using patterns to find a template that matches a given document.
* `trimIndentation` - "intelligently" trim whitespace indentation from the start of each line of a block of text.
* `writeFile` - Write some contents to a file, ensuring the path to the file exists.

#### 模板查找

The template used to render a doc is computed by the `templateFinder`, 
which uses the first match from a set of patterns in a set of folders, provided in the configuration. 

This allows a lot of control to provide generic templates for most situations and specific templates for exceptional cases.

标准模板模式示例：

```js
templateFinder.templatePatterns = [
  '${ doc.template }',
  '${ doc.area }/${ doc.id }.${ doc.docType }.template.html',
  '${ doc.area }/${ doc.id }.template.html',
  '${ doc.area }/${ doc.docType }.template.html',
  '${ doc.id }.${ doc.docType }.template.html',
  '${ doc.id }.template.html',
  '${ doc.docType }.template.html'
]
```
