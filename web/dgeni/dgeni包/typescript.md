
## typescript

### 文件读取器

* at the moment we are not using a filereader but the `readTypeScriptModules` processor to read our modules.

### 处理器

* `readTypeScriptModules` - parse the `sourceFiles` with the help of the `tsParser` service and return a doc
for each exported member. You can either pass an array of strings or an array of objects with `include` and
`exclude` globbing patterns. A mix of both is possible as well.
The processor can be configured to export private
members (marked as `/** @internal */` as well as members starting with an underscore (`_`)) by setting the property
`hidePrivateMembers` to `false`.
Set `sortClassMembers` to `true` to sort instance and static members by name (defaults to order of appearence).
You can ignore special exports by adding strings or regexes to the `ignoreExportsMatching` property (defaults to
`___esModule`.

### 服务

* `convertPrivateClassesToInterfaces` - pass this service a list of exported docs and if it represents a
class that is marked as `/** @internal */` the doc will be converted to represent an interface.
* `tsParser` - uses the typescript compiler and a host created by `createCompilerHost` to actually read
and compile the source files. The docs are created from the symbols read by the typescript program.
* `createCompilerHost` - creates a new compiler host which can, among other things, resolve file paths and
check if files exist
* `getContent` - retrieves the file contents and comments.

### 模板

**This package does not provide any templates nor a `templateEngine` to render templates (use the `nunjucks` package to add this).**

### 标签定义

Please note that at the moment the `@param` documentation is ignored.




