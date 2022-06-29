
## git

This package provides some git and version information to the `renderDocsPocessor` that is available
in the templates. This code as it is was made for the angular.js document generation, including some
custom logic for special versions. However, any of the services can be overridden with custom
behavior.

The git information is made available to templates via the `extraData.git` property. See the section
below to see an example usage.

### 服务

* `decorateVersion` - all semvers are passed through this function so that additional data can before added to them.
* `getPreviousVersions` - pulls versions from git tags of the repository.
* `gitData` - the additional information that is added to the extraData of `renderDocsPocessor`.
* `gitRepoInfo` - the owner and repo of the local git repository.
* `packageInfo` - the contents of the package.json.
* `versionInfo` - aggregated version and git information.

### 使用extraData.git

git/templates/api/api.template.html中的使用示例：

```html+jinja
<a href='https://github.com/{$ git.info.owner $}/{$ git.info.repo $}/tree/{$ git.version.isSnapshot and 'master' or git.version.raw $}/{$ doc.fileInfo.projectRelativePath $}#L{$ doc.startingLine $}' class='view-source pull-right btn btn-primary'>
  <i class="glyphicon glyphicon-zoom-in">&nbsp;</i>View Source
</a>
```
