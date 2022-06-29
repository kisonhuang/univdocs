
## post-process-html

This package provides a HTML post process manager powered by [`rehype`](https://github.com/rehypejs/rehype). It uses the rehype processing engine to manipulate the `renderedContent` HTML via rehype "plugins" that work with HTML ASTs (HASTs).
Read more https://github.com/wooorm/rehype

### 处理器

* `post-process-html` -  Use the rehype processing engine to manipulate the
`renderedContent` HTML via rehype "plugins" that work with HTML ASTs (HASTs).
Each plugin is a factory function that will be called with the "rehype" engine as `this`.
The factory should return a `transform` function that takes a HAST and returns a `boolean` or`undefined`.
The HAST can be mutated by the "transform" function.
If `false` is returned then the processing stops with that plugin.
