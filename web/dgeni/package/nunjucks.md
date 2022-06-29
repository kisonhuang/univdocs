
## nunjucks

This package provides a nunjucks driven implementation of the `templateEngine` required by the
`base` package `renderDocsPocessor`. The "nunjucks" JavaScript template tool-kit to generates HTML
based on the data in each document. We have nunjucks templates, tags and filters that
can render links and text as markdown and will highlight code.

### 服务

* `nunjucks-template-engine` - provide a `templateEngine` that uses the Nunjucks template library to render the documents into text, such as HTML or JS, based on templates.
