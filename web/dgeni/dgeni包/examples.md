
## examples

This package is a mix-in that provides functionality for working with examples in the docs.

Inside your docs you can markup inline-examples such as:

```
Some text before the example

<example name="example-name">
  <file name="index.html">
    <div>The main HTML for the example</div>
  </file>
  <file name="app.js">
    // Some JavaScript code to be included in the example
  </file>
</example>

Some text after the example
```


### 处理器

* `generateExamplesProcessor` - Add new docs to the docs collection for each example in the `examples` service
that will be rendered as files that can be run in the browser, for example as live in-place demos of the
examples or for e2e testing. This processor must be configured with a collection of deployments that tell it
what versions of each example to generate. See the section of **Deployment Configuration** below.
* `parseExamplesProcessor` - Parse the `<example>` tags from the content and add them to the `examples` service
* `generateProtractorTestsProcessor` - Generate a protractor test files from the e2e tests in the examples. This processor
must be configured with a collection of deployments that tell versions of the protractor tests to generate. See the
section of **Deployment Configuration** below.

#### 部署配置

The `generateExamplesProcessor` and `generateProtractorTestsProcessor` processors have a *required* property called `deployments`.
This property should be an array of deployment information objects telling the processor what files to generate.

For instance you might have a "debug" deployment that loads angular.js into the example, and also a "default" deployment that
loads angular.min.js into the example. Equally you might have deployments that use JQuery and some that only use Angular's
jqLite.

You can configure this in your package like so:

```js
.config(function(generateExamplesProcessor, generateProtractorTestsProcessor) {
  var deployments = [
    { name: 'debug', ... },
    { name: 'default', ... }
  ];

  generateExamplesProcessor.deployments = deployments;
  generateProtractorTestsProcessor.deployments = deployments;
});
```

A deployment can must have a `name` property and can also include an `examples` property that contains
information about paths and extra files to inject into runtime examples.
Further a protractor test is generated for each deployment and it uses the deployment name to find the
path to the associated example for that deployment.

```js
{
  name: 'default',
  examples: {
    commonFiles: {
      scripts: [ '../../../angular.js' ]
    },
    dependencyPath: '../../../'
  }
}
```

Here you can see we have a `default` deployment that injects the `angular.js` file into all examples,
plus any dependencies referenced in the example itself are made relative to the given `dependencyPath`.

### 内联标签定义

* `runnableExample` - Inject the specified runnable example into the doc


### 服务

* `exampleMap` - a hash map holding each example by id, which is a unique id generated from the name
of the example
