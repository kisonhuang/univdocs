# 安装client-go

## 使用最新版本

使用go1.16+运行：

```sh
go get k8s.io/client-go@latest
```

## 使用特定版本

+ Kubernetes >= v1.17.0 ---> client-go v0.x.y

例如：Kubernetes v1.20.4 ---> k8s.io/client-go@v0.20.4

```sh
go get k8s.io/client-go@v0.20.4
```

+ Kubernetes < v1.17.0 ---> client-go kubernetes-1.x.y

例如：Kubernetes v1.16.3 ---> k8s.io/client-go@kubernetes-1.16.3

```sh
go get k8s.io/client-go@kubernetes-1.16.3
```

## Troubleshooting

### Go versions prior to 1.16

If you get a message like 
`module k8s.io/client-go@latest found (v1.5.2), but does not contain package k8s.io/client-go/...`,
you are likely using a go version prior to 1.16 and must explicitly specify the k8s.io/client-go version you want.
For example:
```sh
go get k8s.io/client-go@v0.20.4
```

### Conflicting requirements for older client-go versions

If you get a message like
`module k8s.io/api@latest found, but does not contain package k8s.io/api/auditregistration/v1alpha1`,
something in your build is likely requiring an old version of `k8s.io/client-go` like `v11.0.0+incompatible`.

First, try to fetch a more recent version. For example:
```sh
go get k8s.io/client-go@v0.20.4
```

If that doesn't resolve the problem, see what is requiring an `...+incompatible` version of client-go,
and update to use a newer version of that library, if possible:
```sh
go mod graph | grep " k8s.io/client-go@"
```

As a last resort, you can force the build to use a specific version of client-go,
even if some of your dependencies still want `...+incompatible` versions. For example:
```sh
go mod edit -replace=k8s.io/client-go=k8s.io/client-go@v0.20.4
go get k8s.io/client-go@v0.20.4
```

### Go modules disabled

If you get a message like `cannot use path@version syntax in GOPATH mode`,
you likely do not have go modules enabled.

Dependency management tools are built into go 1.11+ in the form of 
[go modules](https://github.com/golang/go/wiki/Modules).
These are used by the main Kubernetes repo (>= `v1.15.0`) and 
`client-go` (>= `kubernetes-1.15.0`) to manage dependencies.
If you are using go 1.11 or 1.12 and are working with a project located within `$GOPATH`,
you must opt into using go modules:

```sh
export GO111MODULE=on
```

Ensure your project has a `go.mod` file defined at the root of your project.
If you do not already have one, `go mod init` will create one for you:

```sh
go mod init
```
