# Dgeni包

Dgeni文档生成器使用Dgeni包来根据源代码创建文档。

Dgeni包：
+ base：Dgeni基础处理器。
+ git：提供git和版本信息。
+ jsdoc：解析和提取标签。
+ nunjucks：nunjucks模板渲染引擎，jsdoc中已不再包含，必须显式地添加到配置中，否则将会得到错误：Error: No provider for "templateEngine"! (Resolving: templateEngine)。
+ ngdoc：angular.js的标签定义、处理器和模板，会加载jsdoc和nunjucks包。
+ examples：生成angular.js文档网站中可以运行的示例。
+ dgeni：生成Dgeni包的文档。
+ typescript：解析和提取TypeScript模块的标签。


