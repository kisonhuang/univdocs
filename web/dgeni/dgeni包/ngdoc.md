
## ngdoc

The `ngdoc` Package depends upon the `jsdoc` and `nunjucks` packages. It provides additional support for
non-API documents written in files with `.ngdoc` extension; it also computes additional properties specific
to Angular related code.

### 文件读取器

* `ngdoc` - can pull a single document from an ngdoc content file.

### 处理器

* `filterNgdocsProcessor` -
For AngularJS we are only interested in documents that contain the @ngdoc tag.  This processor
removes docs that do not contain this tag.

* `generateComponentGroupsProcessor` -
Generate documents for each group of components (by type) within a module

* `memberDocsProcessor` - This processor connects docs that are members (properties, methods and events) to
their container docs, removing them from the main docs collection.

* `moduleDocsProcessor` - This processor computes properties for module docs such as `packageName` and
`packageFileName`; it adds modules to the `moduleMap` service and connects all the docs that are in a module
to the module doc in the `components` property

* `providerDocsProcessor` - This processor relates documents about angular services to their corresponding
provider document.


### 标签定义

This package modifies and adds new tag definitions on top of those provided by the `jsdoc` package:
`area`, `element`, `eventType`, `example`, `fullName`, `id`, `module`, `name`, `ngdoc`, `packageName`,
`parent`, `priority`, `restrict`, `scope` and `title`.


### 内联标签定义

* `link` - Process inline link tags (of the form {@link some/uri Some Title}), replacing them with
HTML anchors


### 服务

* `getAliases()` - Get a list of all the aliases that can be made from the provided doc
* `getDocFromAliases()` - Find a document from the `aliasMap` that matches the given alias
* `getLinkInfo()` - Get link information to a document that matches the given url
* `getTypeClass()` - Get a CSS class string for the given type string
* `moduleMap` - A collection of modules keyed on the module id

### 模板

This package provides a set of templates for generating an HTML file for each document: api,
directive, error, filter function, input, module, object, overview, provider, service, type and a
number to support rendering of the runnable examples.

You should be aware that because of the overlap in syntax between Nunjucks bindings and AngularJS
bindings, the ngdoc package changes the default Nunjucks binding tags:

```js
templateEngine.config.tags = {
  variableStart: '{$',
  variableEnd: '$}'
};
```

### 渲染过滤器

* `code` - Render a span of text as code
* `link` - Render a HTML anchor link
* `typeClass` - Render a CSS class for a given type

### 渲染标签

* `code` - Render a block of code
