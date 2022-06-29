
## jsdoc

### 文件读取器

* `jsdoc` - can read documents from jsdoc style comments in source code files.

### 处理器

* `codeNameProcessor` - infer the name of the document from the code following the document in the source file.
* `extractTagsProcessor` - use a `tagExtractor` to extract information from the parsed tags.
* `inlineTagsProcessor` - Search the docs for inline tags that need to have content injected
* `parseTagsProcessor` - use a `tagParser` to parses the jsdoc tags in the document content.

### 标签定义

The `jsdoc` package contains definitions for a number of standard jsdoc tags including: `name`,
`memberof`, `param`, `property`, `returns`, `module`, `description`, `usage`,
`animations`, `constructor`, `class`, `classdesc`, `global`, `namespace`, `method`, `type`,
`kind`, `access`, `public`, `private` and `protected`.

### 服务（标签转换）

This package provides a number of **Transform** services that are used in **Tag Definitions** to transform
the value of the tag from the string in the tag description to something more meaningful in the doc.

* `extractAccessTransform` - extract an access level (e.g. public, protected, private) from tags
  You can configure this transform to register access tags and set the property where access info is written.
  * `extractAccessTransform.allowedTags.set('tagName', [propertValue])` - register a tag that can act as
    as an alias to set an access level. The propertyValue is optional and if not undefined will return this
    value from the transform that will be written to the property. (defaults to `public:undefined`,
    `private:undefined`, `protected:undefined`)
  * `extractAccessTransformImpl.allowedDocTypes.set('docType')` - register a docType that can contain access
    type tags (defaults to "property" and "method")
  * `extractAccessTransformImpl.accessProperty` - specify the property to which to write the access value
    (defaults to "access")
  * `extractAccessTransformImpl.accessTagName` - specify the name of the tag that can hold access values
    (defaults to "access")
* `extractNameTransform` - extract a name from a tag
* `extractTypeTransform` - extract a type from a tag
* `trimWhitespaceTransform` - trim whitespace from before and after the tag value
* `unknownTagTransform` - add an error to the tag if it is unknown
* `wholeTagTransform` - Use the whole tag as the value rather than using a tag property
* `codeNameService` - helper service for `codeNameProcessor`, registers code name matchers and performs
 actual matches against AST tree

### 模板

**This package does not provide any templates nor a `templateEngine` to render templates (use the `nunjucks` package to add this).**

### 标签定义

This package provides a minimal implementation of tags from the JSDoc project. They extract the name
and type from the tag description accordingly but do not fully implement all the JSDoc tag functionality.

### 代码名称匹配器
Matcher performs a search for a suitable code name at the given jsdoc code point (AST node).
`codeNameService` matches AST node name against matcher name and if suitable matcher is found, executes it.

Matcher name consists of `<AstNodeName>` and `NodeMatcher` substrings, i.e. `FunctionExpressionNodeMatcher`
then latter is stripped and matcher is used by the former part, i.e. `FunctionExpression`.

Matcher should accept single argument - node and return either string with name or literal `null`.

匹配器：
+ ArrayExpression
+ ArrowFunctionExpression
+ AssignmentExpression
+ CallExpression
+ ClassDeclaration
+ ExportDefaultDeclaration
+ ExpressionStatement
+ FunctionDeclaration
+ FunctionExpression
+ Identifier
+ Literal
+ MemberExpression
+ MethodDefinition
+ NewExpression
+ ObjectExpression
+ Program
+ Property
+ ReturnStatement
+ ThrowStatement
+ VariableDeclaration
+ VariableDeclarator
