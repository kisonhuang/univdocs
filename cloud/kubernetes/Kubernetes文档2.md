# Kubernetes文档

+ https://kubernetes.io/docs

## 主页

+ https://kubernetes.io/docs/home
+ https://kubernetes.io/docs/home/supported-doc-versions

## 入门

+ https://kubernetes.io/docs/setup

### 学习环境

+ https://kubernetes.io/docs/setup/learning-environment

### 生产环境

+ https://kubernetes.io/docs/setup/production-environment

#### 容器运行时

+ https://kubernetes.io/docs/setup/production-environment/container-runtimes

#### 使用部署工具安装Kubernetes

+ https://kubernetes.io/docs/setup/production-environment/tools

+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/install-kubeadm
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/troubleshooting-kubeadm
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/control-plane-flags
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/ha-topology
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/high-availability
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/setup-ha-etcd-with-kubeadm
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/kubelet-integration
+ https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/dual-stack-support

+ https://kubernetes.io/docs/setup/production-environment/tools/kops
+ https://kubernetes.io/docs/setup/production-environment/tools/kubespray

#### 云厂商的解决方案

+ https://kubernetes.io/docs/setup/production-environment/turnkey-solutions

### 最佳实践

+ https://kubernetes.io/docs/setup/best-practices
+ https://kubernetes.io/docs/setup/best-practices/cluster-large
+ https://kubernetes.io/docs/setup/best-practices/multiple-zones
+ https://kubernetes.io/docs/setup/best-practices/node-conformance
+ https://kubernetes.io/docs/setup/best-practices/enforcing-pod-security-standards
+ https://kubernetes.io/docs/setup/best-practices/certificates

## 概念

+ https://kubernetes.io/docs/concepts

### 概述

+ https://kubernetes.io/docs/concepts/overview

+ https://kubernetes.io/docs/concepts/overview/what-is-kubernetes
+ https://kubernetes.io/docs/concepts/overview/components
+ https://kubernetes.io/docs/concepts/overview/kubernetes-api

+ https://kubernetes.io/docs/concepts/overview/working-with-objects
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/kubernetes-objects
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/object-management
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/names
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/labels
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/field-selectors
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/finalizers
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/owners-dependents
+ https://kubernetes.io/docs/concepts/overview/working-with-objects/common-labels

### 集群架构

+ https://kubernetes.io/docs/concepts/architecture
+ https://kubernetes.io/docs/concepts/architecture/nodes
+ https://kubernetes.io/docs/concepts/architecture/control-plane-node-communication
+ https://kubernetes.io/docs/concepts/architecture/controller
+ https://kubernetes.io/docs/concepts/architecture/cloud-controller
+ https://kubernetes.io/docs/concepts/architecture/cri
+ https://kubernetes.io/docs/concepts/architecture/garbage-collection

### 容器

+ https://kubernetes.io/docs/concepts/containers
+ https://kubernetes.io/docs/concepts/containers/images
+ https://kubernetes.io/docs/concepts/containers/container-environment
+ https://kubernetes.io/docs/concepts/containers/runtime-class
+ https://kubernetes.io/docs/concepts/containers/container-lifecycle-hooks

### Windows中的Kubernetes

+ https://kubernetes.io/docs/concepts/windows
+ https://kubernetes.io/docs/concepts/windows/intro
+ https://kubernetes.io/docs/concepts/windows/user-guide

### 工作负载

+ https://kubernetes.io/docs/concepts/workloads

+ https://kubernetes.io/docs/concepts/workloads/pods
+ https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle
+ https://kubernetes.io/docs/concepts/workloads/pods/init-containers
+ https://kubernetes.io/docs/concepts/workloads/pods/pod-topology-spread-constraints
+ https://kubernetes.io/docs/concepts/workloads/pods/disruptions
+ https://kubernetes.io/docs/concepts/workloads/pods/ephemeral-containers

+ https://kubernetes.io/docs/concepts/workloads/controllers
+ https://kubernetes.io/docs/concepts/workloads/controllers/deployment
+ https://kubernetes.io/docs/concepts/workloads/controllers/replicaset
+ https://kubernetes.io/docs/concepts/workloads/controllers/statefulset
+ https://kubernetes.io/docs/concepts/workloads/controllers/daemonset
+ https://kubernetes.io/docs/concepts/workloads/controllers/job
+ https://kubernetes.io/docs/concepts/workloads/controllers/ttlafterfinished
+ https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs
+ https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller

### 服务、负载均衡和网络

+ https://kubernetes.io/docs/concepts/services-networking
+ https://kubernetes.io/docs/concepts/services-networking/service
+ https://kubernetes.io/docs/concepts/services-networking/service-topology
+ https://kubernetes.io/docs/concepts/services-networking/dns-pod-service
+ https://kubernetes.io/docs/concepts/services-networking/connect-applications-service
+ https://kubernetes.io/docs/concepts/services-networking/ingress
+ https://kubernetes.io/docs/concepts/services-networking/ingress-controllers
+ https://kubernetes.io/docs/concepts/services-networking/endpoint-slices
+ https://kubernetes.io/docs/concepts/services-networking/service-traffic-policy
+ https://kubernetes.io/docs/concepts/services-networking/topology-aware-hints
+ https://kubernetes.io/docs/concepts/services-networking/network-policies
+ https://kubernetes.io/docs/concepts/services-networking/dual-stack
+ https://kubernetes.io/docs/concepts/services-networking/windows-networking

### 存储

+ https://kubernetes.io/docs/concepts/storage
+ https://kubernetes.io/docs/concepts/storage/volumes
+ https://kubernetes.io/docs/concepts/storage/persistent-volumes
+ https://kubernetes.io/docs/concepts/storage/projected-volumes
+ https://kubernetes.io/docs/concepts/storage/ephemeral-volumes
+ https://kubernetes.io/docs/concepts/storage/storage-classes
+ https://kubernetes.io/docs/concepts/storage/dynamic-provisioning
+ https://kubernetes.io/docs/concepts/storage/volume-snapshots
+ https://kubernetes.io/docs/concepts/storage/volume-snapshot-classes
+ https://kubernetes.io/docs/concepts/storage/volume-pvc-datasource
+ https://kubernetes.io/docs/concepts/storage/storage-capacity
+ https://kubernetes.io/docs/concepts/storage/storage-limits
+ https://kubernetes.io/docs/concepts/storage/volume-health-monitoring
+ https://kubernetes.io/docs/concepts/storage/windows-storage

### 配置

+ https://kubernetes.io/docs/concepts/configuration
+ https://kubernetes.io/docs/concepts/configuration/overview
+ https://kubernetes.io/docs/concepts/configuration/configmap
+ https://kubernetes.io/docs/concepts/configuration/secret
+ https://kubernetes.io/docs/concepts/configuration/manage-resources-containers
+ https://kubernetes.io/docs/concepts/configuration/organize-cluster-access-kubeconfig
+ https://kubernetes.io/docs/concepts/configuration/windows-resource-management

### 安全

+ https://kubernetes.io/docs/concepts/security
+ https://kubernetes.io/docs/concepts/security/overview
+ https://kubernetes.io/docs/concepts/security/pod-security-standards
+ https://kubernetes.io/docs/concepts/security/pod-security-admission
+ https://kubernetes.io/docs/concepts/security/pod-security-policy
+ https://kubernetes.io/docs/concepts/security/windows-security
+ https://kubernetes.io/docs/concepts/security/controlling-access
+ https://kubernetes.io/docs/concepts/security/rbac-good-practices

### 策略

+ https://kubernetes.io/docs/concepts/policy
+ https://kubernetes.io/docs/concepts/policy/limit-range
+ https://kubernetes.io/docs/concepts/policy/resource-quotas
+ https://kubernetes.io/docs/concepts/policy/pid-limiting
+ https://kubernetes.io/docs/concepts/policy/node-resource-managers

### 调度、抢占和驱逐

+ https://kubernetes.io/docs/concepts/scheduling-eviction
+ https://kubernetes.io/docs/concepts/scheduling-eviction/kube-scheduler
+ https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node
+ https://kubernetes.io/docs/concepts/scheduling-eviction/pod-overhead
+ https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration
+ https://kubernetes.io/docs/concepts/scheduling-eviction/pod-priority-preemption
+ https://kubernetes.io/docs/concepts/scheduling-eviction/node-pressure-eviction
+ https://kubernetes.io/docs/concepts/scheduling-eviction/api-eviction
+ https://kubernetes.io/docs/concepts/scheduling-eviction/resource-bin-packing
+ https://kubernetes.io/docs/concepts/scheduling-eviction/scheduling-framework
+ https://kubernetes.io/docs/concepts/scheduling-eviction/scheduler-perf-tuning

### 集群管理

+ https://kubernetes.io/docs/concepts/cluster-administration
+ https://kubernetes.io/docs/concepts/cluster-administration/certificates
+ https://kubernetes.io/docs/concepts/cluster-administration/manage-deployment
+ https://kubernetes.io/docs/concepts/cluster-administration/networking
+ https://kubernetes.io/docs/concepts/cluster-administration/logging
+ https://kubernetes.io/docs/concepts/cluster-administration/system-metrics
+ https://kubernetes.io/docs/concepts/cluster-administration/system-logs
+ https://kubernetes.io/docs/concepts/cluster-administration/system-traces
+ https://kubernetes.io/docs/concepts/cluster-administration/proxies
+ https://kubernetes.io/docs/concepts/cluster-administration/flow-control
+ https://kubernetes.io/docs/concepts/cluster-administration/addons

### 扩展Kubernetes

+ https://kubernetes.io/docs/concepts/extend-kubernetes
+ https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension
+ https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources
+ https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/apiserver-aggregation
+ https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net
+ https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/network-plugins
+ https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/device-plugins
+ https://kubernetes.io/docs/concepts/extend-kubernetes/operator
+ https://kubernetes.io/docs/concepts/extend-kubernetes/service-catalog

## 任务

+ https://kubernetes.io/docs/tasks

### 安装工具

+ https://kubernetes.io/docs/tasks/tools

+ https://kubernetes.io/docs/tasks/tools/install-kubectl-linux
+ https://kubernetes.io/docs/tasks/tools/install-kubectl-macos
+ https://kubernetes.io/docs/tasks/tools/install-kubectl-windows

### 管理集群

+ https://kubernetes.io/docs/tasks/administer-cluster

+ https://kubernetes.io/docs/tasks/administer-cluster/kubeadm
+ https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/kubeadm-certs
+ kubernetes/安装/配置cgroup驱动.md
+ https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/kubeadm-reconfigure
+ https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/kubeadm-upgrade
+ https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/adding-windows-nodes
+ https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/upgrading-windows-nodes

+ https://kubernetes.io/docs/tasks/administer-cluster/migrating-from-dockershim
+ https://kubernetes.io/docs/tasks/administer-cluster/migrating-from-dockershim/change-runtime-containerd
+ https://kubernetes.io/docs/tasks/administer-cluster/migrating-from-dockershim/migrate-dockershim-dockerd
+ https://kubernetes.io/docs/tasks/administer-cluster/migrating-from-dockershim/find-out-runtime-you-use
+ https://kubernetes.io/docs/tasks/administer-cluster/migrating-from-dockershim/troubleshooting-cni-plugin-related-errors
+ https://kubernetes.io/docs/tasks/administer-cluster/migrating-from-dockershim/check-if-dockershim-removal-affects-you
+ https://kubernetes.io/docs/tasks/administer-cluster/migrating-from-dockershim/migrating-telemetry-and-security-agents

+ https://kubernetes.io/docs/tasks/administer-cluster/certificates

+ https://kubernetes.io/docs/tasks/administer-cluster/manage-resources
+ https://kubernetes.io/docs/tasks/administer-cluster/manage-resources/memory-default-namespace
+ https://kubernetes.io/docs/tasks/administer-cluster/manage-resources/cpu-default-namespace
+ https://kubernetes.io/docs/tasks/administer-cluster/manage-resources/memory-constraint-namespace
+ https://kubernetes.io/docs/tasks/administer-cluster/manage-resources/cpu-constraint-namespace
+ https://kubernetes.io/docs/tasks/administer-cluster/manage-resources/quota-memory-cpu-namespace
+ https://kubernetes.io/docs/tasks/administer-cluster/manage-resources/quota-pod-namespace

+ https://kubernetes.io/docs/tasks/administer-cluster/network-policy-provider
+ https://kubernetes.io/docs/tasks/administer-cluster/network-policy-provider/antrea-network-policy
+ https://kubernetes.io/docs/tasks/administer-cluster/network-policy-provider/calico-network-policy
+ https://kubernetes.io/docs/tasks/administer-cluster/network-policy-provider/cilium-network-policy
+ https://kubernetes.io/docs/tasks/administer-cluster/network-policy-provider/kube-router-network-policy
+ https://kubernetes.io/docs/tasks/administer-cluster/network-policy-provider/romana-network-policy
+ https://kubernetes.io/docs/tasks/administer-cluster/network-policy-provider/weave-network-policy

+ https://kubernetes.io/docs/tasks/administer-cluster/access-cluster-api
+ https://kubernetes.io/docs/tasks/administer-cluster/extended-resource-node
+ https://kubernetes.io/docs/tasks/administer-cluster/dns-horizontal-autoscaling
+ https://kubernetes.io/docs/tasks/administer-cluster/change-default-storage-class
+ https://kubernetes.io/docs/tasks/administer-cluster/change-pv-reclaim-policy
+ https://kubernetes.io/docs/tasks/administer-cluster/running-cloud-controller
+ https://kubernetes.io/docs/tasks/administer-cluster/quota-api-object
+ https://kubernetes.io/docs/tasks/administer-cluster/cpu-management-policies
+ https://kubernetes.io/docs/tasks/administer-cluster/topology-manager
+ https://kubernetes.io/docs/tasks/administer-cluster/dns-custom-nameservers
+ https://kubernetes.io/docs/tasks/administer-cluster/dns-debugging-resolution
+ https://kubernetes.io/docs/tasks/administer-cluster/declare-network-policy
+ https://kubernetes.io/docs/tasks/administer-cluster/developing-cloud-controller-manager
+ https://kubernetes.io/docs/tasks/administer-cluster/enable-disable-api
+ https://kubernetes.io/docs/tasks/administer-cluster/enabling-service-topology
+ https://kubernetes.io/docs/tasks/administer-cluster/encrypt-data
+ https://kubernetes.io/docs/tasks/administer-cluster/guaranteed-scheduling-critical-addon-pods
+ https://kubernetes.io/docs/tasks/administer-cluster/ip-masq-agent
+ https://kubernetes.io/docs/tasks/administer-cluster/limit-storage-consumption
+ https://kubernetes.io/docs/tasks/administer-cluster/controller-manager-leader-migration
+ https://kubernetes.io/docs/tasks/administer-cluster/namespaces-walkthrough
+ https://kubernetes.io/docs/tasks/administer-cluster/configure-upgrade-etcd
+ https://kubernetes.io/docs/tasks/administer-cluster/reconfigure-kubelet
+ https://kubernetes.io/docs/tasks/administer-cluster/reserve-compute-resources
+ https://kubernetes.io/docs/tasks/administer-cluster/kubelet-in-userns
+ https://kubernetes.io/docs/tasks/administer-cluster/safely-drain-node
+ https://kubernetes.io/docs/tasks/administer-cluster/securing-a-cluster
+ https://kubernetes.io/docs/tasks/administer-cluster/kubelet-config-file
+ https://kubernetes.io/docs/tasks/administer-cluster/namespaces
+ https://kubernetes.io/docs/tasks/administer-cluster/cluster-upgrade
+ https://kubernetes.io/docs/tasks/administer-cluster/use-cascading-deletion
+ https://kubernetes.io/docs/tasks/administer-cluster/kms-provider
+ https://kubernetes.io/docs/tasks/administer-cluster/coredns
+ https://kubernetes.io/docs/tasks/administer-cluster/nodelocaldns
+ https://kubernetes.io/docs/tasks/administer-cluster/sysctl-cluster
+ https://kubernetes.io/docs/tasks/administer-cluster/memory-manager
+ https://kubernetes.io/docs/tasks/administer-cluster/verify-signed-images

### 配置Pod和容器

+ https://kubernetes.io/docs/tasks/configure-pod-container
+ https://kubernetes.io/docs/tasks/configure-pod-container/assign-memory-resource
+ https://kubernetes.io/docs/tasks/configure-pod-container/assign-cpu-resource
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-gmsa
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-runasusername
+ https://kubernetes.io/docs/tasks/configure-pod-container/create-hostprocess-pod
+ https://kubernetes.io/docs/tasks/configure-pod-container/quality-service-pod
+ https://kubernetes.io/docs/tasks/configure-pod-container/extended-resource
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-volume-storage
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-persistent-volume-storage
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-projected-volume-storage
+ https://kubernetes.io/docs/tasks/configure-pod-container/security-context
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-service-account
+ https://kubernetes.io/docs/tasks/configure-pod-container/pull-image-private-registry
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes
+ https://kubernetes.io/docs/tasks/configure-pod-container/assign-pods-nodes
+ https://kubernetes.io/docs/tasks/configure-pod-container/assign-pods-nodes-using-node-affinity
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-initialization
+ https://kubernetes.io/docs/tasks/configure-pod-container/attach-handler-lifecycle-event
+ https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap
+ https://kubernetes.io/docs/tasks/configure-pod-container/share-process-namespace
+ https://kubernetes.io/docs/tasks/configure-pod-container/static-pod
+ https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes
+ https://kubernetes.io/docs/tasks/configure-pod-container/enforce-standards-admission-controller
+ https://kubernetes.io/docs/tasks/configure-pod-container/enforce-standards-namespace-labels
+ https://kubernetes.io/docs/tasks/configure-pod-container/migrate-from-psp

### 监控、日志和调试

+ https://kubernetes.io/docs/tasks/debug
+ https://kubernetes.io/docs/tasks/debug/debug-application
+ https://kubernetes.io/docs/tasks/debug/debug-application/debug-pods
+ https://kubernetes.io/docs/tasks/debug/debug-application/debug-service
+ https://kubernetes.io/docs/tasks/debug/debug-application/debug-statefulset
+ https://kubernetes.io/docs/tasks/debug/debug-application/debug-init-containers
+ https://kubernetes.io/docs/tasks/debug/debug-application/debug-running-pod
+ https://kubernetes.io/docs/tasks/debug/debug-application/determine-reason-pod-failure
+ https://kubernetes.io/docs/tasks/debug/debug-application/get-shell-running-container
+ https://kubernetes.io/docs/tasks/debug/debug-cluster
+ https://kubernetes.io/docs/tasks/debug/debug-cluster/resource-metrics-pipeline
+ https://kubernetes.io/docs/tasks/debug/debug-cluster/resource-usage-monitoring
+ https://kubernetes.io/docs/tasks/debug/debug-cluster/monitor-node-health
+ https://kubernetes.io/docs/tasks/debug/debug-cluster/crictl
+ https://kubernetes.io/docs/tasks/debug/debug-cluster/audit
+ https://kubernetes.io/docs/tasks/debug/debug-cluster/local-debugging
+ https://kubernetes.io/docs/tasks/debug/debug-cluster/windows

### 管理Kubernetes对象

+ https://kubernetes.io/docs/tasks/manage-kubernetes-objects
+ https://kubernetes.io/docs/tasks/manage-kubernetes-objects/declarative-config
+ https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization
+ https://kubernetes.io/docs/tasks/manage-kubernetes-objects/imperative-command
+ https://kubernetes.io/docs/tasks/manage-kubernetes-objects/imperative-config
+ https://kubernetes.io/docs/tasks/manage-kubernetes-objects/update-api-object-kubectl-patch

### 管理密钥

+ https://kubernetes.io/docs/tasks/configmap-secret
+ https://kubernetes.io/docs/tasks/configmap-secret/managing-secret-using-kubectl
+ https://kubernetes.io/docs/tasks/configmap-secret/managing-secret-using-config-file
+ https://kubernetes.io/docs/tasks/configmap-secret/managing-secret-using-kustomize

### 把数据注入应用程序

+ https://kubernetes.io/docs/tasks/inject-data-application
+ https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container
+ https://kubernetes.io/docs/tasks/inject-data-application/define-interdependent-environment-variables
+ https://kubernetes.io/docs/tasks/inject-data-application/define-environment-variable-container
+ https://kubernetes.io/docs/tasks/inject-data-application/environment-variable-expose-pod-information
+ https://kubernetes.io/docs/tasks/inject-data-application/downward-api-volume-expose-pod-information
+ https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure

### 运行应用程序

+ https://kubernetes.io/docs/tasks/run-application
+ https://kubernetes.io/docs/tasks/run-application/run-stateless-application-deployment
+ https://kubernetes.io/docs/tasks/run-application/run-single-instance-stateful-application
+ https://kubernetes.io/docs/tasks/run-application/run-replicated-stateful-application
+ https://kubernetes.io/docs/tasks/run-application/scale-stateful-set
+ https://kubernetes.io/docs/tasks/run-application/delete-stateful-set
+ https://kubernetes.io/docs/tasks/run-application/force-delete-stateful-set-pod
+ https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale
+ https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale-walkthrough
+ https://kubernetes.io/docs/tasks/run-application/configure-pdb
+ https://kubernetes.io/docs/tasks/run-application/access-api-from-pod

### 运行任务

+ https://kubernetes.io/docs/tasks/job
+ https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs
+ https://kubernetes.io/docs/tasks/job/coarse-parallel-processing-work-queue
+ https://kubernetes.io/docs/tasks/job/fine-parallel-processing-work-queue
+ https://kubernetes.io/docs/tasks/job/indexed-parallel-processing-static
+ https://kubernetes.io/docs/tasks/job/parallel-processing-expansion

### 访问集群中的应用程序

+ https://kubernetes.io/docs/tasks/access-application-cluster
+ https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard
+ https://kubernetes.io/docs/tasks/access-application-cluster/access-cluster
+ https://kubernetes.io/docs/tasks/access-application-cluster/configure-access-multiple-clusters
+ https://kubernetes.io/docs/tasks/access-application-cluster/port-forward-access-application-cluster
+ https://kubernetes.io/docs/tasks/access-application-cluster/service-access-application-cluster
+ https://kubernetes.io/docs/tasks/access-application-cluster/connecting-frontend-backend
+ https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer
+ https://kubernetes.io/docs/tasks/access-application-cluster/list-all-running-container-images
+ https://kubernetes.io/docs/tasks/access-application-cluster/ingress-minikube
+ https://kubernetes.io/docs/tasks/access-application-cluster/communicate-containers-same-pod-shared-volume
+ https://kubernetes.io/docs/tasks/access-application-cluster/configure-dns-cluster
+ https://kubernetes.io/docs/tasks/access-application-cluster/access-cluster-services

### 扩展Kubernetes

+ https://kubernetes.io/docs/tasks/extend-kubernetes
+ https://kubernetes.io/docs/tasks/extend-kubernetes/configure-aggregation-layer
+ https://kubernetes.io/docs/tasks/extend-kubernetes/custom-resources
+ https://kubernetes.io/docs/tasks/extend-kubernetes/custom-resources/custom-resource-definitions
+ https://kubernetes.io/docs/tasks/extend-kubernetes/custom-resources/custom-resource-definition-versioning
+ https://kubernetes.io/docs/tasks/extend-kubernetes/setup-extension-api-server
+ https://kubernetes.io/docs/tasks/extend-kubernetes/configure-multiple-schedulers
+ https://kubernetes.io/docs/tasks/extend-kubernetes/http-proxy-access-api
+ https://kubernetes.io/docs/tasks/extend-kubernetes/socks5-proxy-access-api
+ https://kubernetes.io/docs/tasks/extend-kubernetes/setup-konnectivity

### TLS

+ https://kubernetes.io/docs/tasks/tls
+ https://kubernetes.io/docs/tasks/tls/certificate-rotation
+ https://kubernetes.io/docs/tasks/tls/managing-tls-in-a-cluster
+ https://kubernetes.io/docs/tasks/tls/manual-rotation-of-ca-certificates

### 管理集群的守护进程

+ https://kubernetes.io/docs/tasks/manage-daemon
+ https://kubernetes.io/docs/tasks/manage-daemon/update-daemon-set
+ https://kubernetes.io/docs/tasks/manage-daemon/rollback-daemon-set

### 服务目录

+ https://kubernetes.io/docs/tasks/service-catalog
+ https://kubernetes.io/docs/tasks/service-catalog/install-service-catalog-using-helm
+ https://kubernetes.io/docs/tasks/service-catalog/install-service-catalog-using-sc

### 网络

+ https://kubernetes.io/docs/tasks/network
+ https://kubernetes.io/docs/tasks/network/customize-hosts-file-for-pods
+ https://kubernetes.io/docs/tasks/network/validate-dual-stack

### 配置kubelet镜像凭证提供器

+ https://kubernetes.io/docs/tasks/kubelet-credential-provider/kubelet-credential-provider

### 使用插件扩展kubectl

+ https://kubernetes.io/docs/tasks/extend-kubectl/kubectl-plugins

### 管理HugePage

+ https://kubernetes.io/docs/tasks/manage-hugepages/scheduling-hugepages

### 调度GPU

+ https://kubernetes.io/docs/tasks/manage-gpus/scheduling-gpus

## 教程

+ https://kubernetes.io/docs/tutorials

### Minikube

+ https://kubernetes.io/docs/tutorials/hello-minikube

### Kubernetes基础

+ https://kubernetes.io/docs/tutorials/kubernetes-basics

+ https://kubernetes.io/docs/tutorials/kubernetes-basics/create-cluster
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/create-cluster/cluster-intro
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/create-cluster/cluster-interactive

+ https://kubernetes.io/docs/tutorials/kubernetes-basics/deploy-app
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/deploy-app/deploy-intro
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/deploy-app/deploy-interactive

+ https://kubernetes.io/docs/tutorials/kubernetes-basics/explore
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/explore/explore-intro
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/explore/explore-interactive

+ https://kubernetes.io/docs/tutorials/kubernetes-basics/expose
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/expose/expose-intro
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/expose/expose-interactive

+ https://kubernetes.io/docs/tutorials/kubernetes-basics/scale
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/scale/scale-intro
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/scale/scale-interactive

+ https://kubernetes.io/docs/tutorials/kubernetes-basics/update
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/update/update-intro
+ https://kubernetes.io/docs/tutorials/kubernetes-basics/update/update-interactive

### 配置

+ https://kubernetes.io/docs/tutorials/configuration
+ https://kubernetes.io/docs/tutorials/configuration/configure-java-microservice
+ https://kubernetes.io/docs/tutorials/configuration/configure-java-microservice/configure-java-microservice
+ https://kubernetes.io/docs/tutorials/configuration/configure-java-microservice/configure-java-microservice-interactive
+ https://kubernetes.io/docs/tutorials/configuration/configure-redis-using-configmap

### 安全

+ https://kubernetes.io/docs/tutorials/security
+ https://kubernetes.io/docs/tutorials/security/cluster-level-pss
+ https://kubernetes.io/docs/tutorials/security/ns-level-pss
+ https://kubernetes.io/docs/tutorials/security/apparmor
+ https://kubernetes.io/docs/tutorials/security/seccomp

### 无状态应用程序

+ https://kubernetes.io/docs/tutorials/stateless-application
+ https://kubernetes.io/docs/tutorials/stateless-application/expose-external-ip-address
+ https://kubernetes.io/docs/tutorials/stateless-application/guestbook

### 有状态应用程序

+ https://kubernetes.io/docs/tutorials/stateful-application
+ https://kubernetes.io/docs/tutorials/stateful-application/basic-stateful-set
+ https://kubernetes.io/docs/tutorials/stateful-application/mysql-wordpress-persistent-volume
+ https://kubernetes.io/docs/tutorials/stateful-application/cassandra
+ https://kubernetes.io/docs/tutorials/stateful-application/zookeeper

### 服务

+ https://kubernetes.io/docs/tutorials/services
+ https://kubernetes.io/docs/tutorials/services/source-ip

## 参考

+ https://kubernetes.io/docs/reference

### 术语
 
+ https://kubernetes.io/docs/reference/glossary

### 使用API

+ https://kubernetes.io/docs/reference/using-api
+ https://kubernetes.io/docs/reference/using-api/api-concepts
+ https://kubernetes.io/docs/reference/using-api/server-side-apply
+ https://kubernetes.io/docs/reference/using-api/client-libraries
+ https://kubernetes.io/docs/reference/using-api/deprecation-policy
+ https://kubernetes.io/docs/reference/using-api/deprecation-guide
+ https://kubernetes.io/docs/reference/using-api/health-checks

### API访问控制

+ https://kubernetes.io/docs/reference/access-authn-authz
+ https://kubernetes.io/docs/reference/access-authn-authz/authentication
+ https://kubernetes.io/docs/reference/access-authn-authz/bootstrap-tokens
+ https://kubernetes.io/docs/reference/access-authn-authz/certificate-signing-requests
+ https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers
+ https://kubernetes.io/docs/reference/access-authn-authz/extensible-admission-controllers
+ https://kubernetes.io/docs/reference/access-authn-authz/service-accounts-admin
+ https://kubernetes.io/docs/reference/access-authn-authz/authorization
+ https://kubernetes.io/docs/reference/access-authn-authz/rbac
+ https://kubernetes.io/docs/reference/access-authn-authz/abac
+ https://kubernetes.io/docs/reference/access-authn-authz/node
+ https://kubernetes.io/docs/reference/access-authn-authz/psp-to-pod-security-standards
+ https://kubernetes.io/docs/reference/access-authn-authz/webhook
+ https://kubernetes.io/docs/reference/access-authn-authz/kubelet-authn-authz
+ https://kubernetes.io/docs/reference/access-authn-authz/kubelet-tls-bootstrapping

### 常见标签、注解和污点

+ https://kubernetes.io/docs/reference/labels-annotations-taints
+ https://kubernetes.io/docs/reference/labels-annotations-taints/audit-annotations

### v1.22 API参考

+ https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.24

### API参考

+ https://kubernetes.io/docs/reference/kubernetes-api

#### 工作负载

+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/pod-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/pod-template-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/replication-controller-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/replica-set-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/deployment-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/stateful-set-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/controller-revision-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/daemon-set-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/job-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/cron-job-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/horizontal-pod-autoscaler-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/horizontal-pod-autoscaler-v2
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/horizontal-pod-autoscaler-v2beta2
+ https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/priority-class-v1

#### 服务

+ https://kubernetes.io/docs/reference/kubernetes-api/service-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/service-resources/service-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/service-resources/endpoints-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/service-resources/endpoint-slice-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/service-resources/ingress-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/service-resources/ingress-class-v1

#### 配置和存储

+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/config-map-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/secret-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/volume
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-claim-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/storage-class-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/volume-attachment-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-driver-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-node-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-storage-capacity-v1

#### 认证

+ https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/service-account-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/token-request-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/token-review-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/certificate-signing-request-v1

#### 授权

+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/local-subject-access-review-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/self-subject-access-review-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/self-subject-rules-review-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/subject-access-review-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/cluster-role-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/cluster-role-binding-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/role-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/role-binding-v1

#### 策略

+ https://kubernetes.io/docs/reference/kubernetes-api/policy-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/limit-range-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/resource-quota-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/network-policy-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/pod-disruption-budget-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/pod-security-policy-v1beta1

#### 扩展

+ https://kubernetes.io/docs/reference/kubernetes-api/extend-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/extend-resources/custom-resource-definition-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/extend-resources/mutating-webhook-configuration-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/extend-resources/validating-webhook-configuration-v1

#### 集群

+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/node-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/namespace-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/event-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/api-service-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/lease-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/runtime-class-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/flow-schema-v1beta2
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/priority-level-configuration-v1beta2
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/binding-v1
+ https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/component-status-v1

#### 通用定义

+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/delete-options
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/label-selector
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/list-meta
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/local-object-reference
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/node-selector-requirement
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/object-field-selector
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/object-meta
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/object-reference
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/patch
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/quantity
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/resource-field-selector
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/status
+ https://kubernetes.io/docs/reference/kubernetes-api/common-definitions/typed-local-object-reference

#### 通用参数

+ https://kubernetes.io/docs/reference/kubernetes-api/common-parameters/common-parameters

### 问题和安全

+ https://kubernetes.io/docs/reference/issues-security
+ https://kubernetes.io/docs/reference/issues-security/issues
+ https://kubernetes.io/docs/reference/issues-security/security

### 节点参考信息

+ https://kubernetes.io/docs/reference/node
+ https://kubernetes.io/docs/reference/node/topics-on-dockershim-and-cri-compatible-runtimes

### 端口和协议

+ https://kubernetes.io/docs/reference/ports-and-protocols

### 安装工具

+ https://kubernetes.io/docs/reference/setup-tools
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-init
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-join
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-upgrade
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-config
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-reset
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-token
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-version
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-alpha
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-certs
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-init-phase
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-join-phase
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-kubeconfig
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-reset-phase
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/kubeadm-upgrade-phase
+ https://kubernetes.io/docs/reference/setup-tools/kubeadm/implementation-details

### kubectl

+ https://kubernetes.io/docs/reference/kubectl
+ https://kubernetes.io/docs/reference/kubectl/cheatsheet
+ https://kubernetes.io/docs/reference/kubectl/kubectl-cmds
+ https://kubernetes.io/docs/reference/kubectl/kubectl
+ https://kubernetes.io/docs/reference/kubectl/jsonpath
+ https://kubernetes.io/docs/reference/kubectl/docker-cli-to-kubectl
+ https://kubernetes.io/docs/reference/kubectl/conventions

### 组件工具

+ https://kubernetes.io/docs/reference/command-line-tools-reference
+ https://kubernetes.io/docs/reference/command-line-tools-reference/feature-gates
+ https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet
+ https://kubernetes.io/docs/reference/command-line-tools-reference/kube-apiserver
+ https://kubernetes.io/docs/reference/command-line-tools-reference/kube-controller-manager
+ https://kubernetes.io/docs/reference/command-line-tools-reference/kube-proxy
+ https://kubernetes.io/docs/reference/command-line-tools-reference/kube-scheduler

### 配置API

+ https://kubernetes.io/docs/reference/config-api
+ https://kubernetes.io/docs/reference/config-api/client-authentication.v1
+ https://kubernetes.io/docs/reference/config-api/client-authentication.v1beta1
+ https://kubernetes.io/docs/reference/config-api/apiserver-eventratelimit.v1alpha1
+ https://kubernetes.io/docs/reference/config-api/imagepolicy.v1alpha1
+ https://kubernetes.io/docs/reference/config-api/apiserver-audit.v1
+ https://kubernetes.io/docs/reference/config-api/apiserver-config.v1
+ https://kubernetes.io/docs/reference/config-api/apiserver-config.v1alpha1
+ https://kubernetes.io/docs/reference/config-api/apiserver-encryption.v1
+ https://kubernetes.io/docs/reference/config-api/kube-proxy-config.v1alpha1
+ https://kubernetes.io/docs/reference/config-api/kube-scheduler-config.v1beta2
+ https://kubernetes.io/docs/reference/config-api/kube-scheduler-config.v1beta3
+ https://kubernetes.io/docs/reference/config-api/kubeadm-config.v1beta2
+ https://kubernetes.io/docs/reference/config-api/kubeadm-config.v1beta3
+ https://kubernetes.io/docs/reference/config-api/kubelet-config.v1alpha1
+ https://kubernetes.io/docs/reference/config-api/kubelet-config.v1beta1
+ https://kubernetes.io/docs/reference/config-api/kubelet-credentialprovider.v1alpha1
+ https://kubernetes.io/docs/reference/config-api/kubelet-credentialprovider.v1beta1
+ https://kubernetes.io/docs/reference/config-api/apiserver-webhookadmission.v1

### 调度

+ https://kubernetes.io/docs/reference/scheduling
+ https://kubernetes.io/docs/reference/scheduling/config
+ https://kubernetes.io/docs/reference/scheduling/policies

### 其他工具

+ https://kubernetes.io/docs/reference/tools
+ https://kubernetes.io/docs/reference/tools/map-crictl-dockercli

## 贡献

+ https://kubernetes.io/docs/contribute

### 建议改进内容

+ https://kubernetes.io/docs/contribute/suggest-improvements

### 贡献新的内容

+ https://kubernetes.io/docs/contribute/new-content
+ https://kubernetes.io/docs/contribute/new-content/open-a-pr
+ https://kubernetes.io/docs/contribute/new-content/new-features
+ https://kubernetes.io/docs/contribute/new-content/blogs-case-studies

### 检查修改

+ https://kubernetes.io/docs/contribute/review
+ https://kubernetes.io/docs/contribute/review/reviewing-prs
+ https://kubernetes.io/docs/contribute/review/for-approvers

### 本地化Kubernetes文档

+ https://kubernetes.io/docs/contribute/localization

### 参与SIG文档

+ https://kubernetes.io/docs/contribute/participate
+ https://kubernetes.io/docs/contribute/participate/roles-and-responsibilities
+ https://kubernetes.io/docs/contribute/participate/pr-wranglers

### 文档风格概述

+ https://kubernetes.io/docs/contribute/style
+ https://kubernetes.io/docs/contribute/style/content-guide
+ https://kubernetes.io/docs/contribute/style/style-guide
+ https://kubernetes.io/docs/contribute/style/diagram-guide
+ https://kubernetes.io/docs/contribute/style/write-new-topic
+ https://kubernetes.io/docs/contribute/style/page-content-types
+ https://kubernetes.io/docs/contribute/style/content-organization
+ https://kubernetes.io/docs/contribute/style/hugo-shortcodes

### 参考文档概述

+ https://kubernetes.io/docs/contribute/generate-ref-docs
+ https://kubernetes.io/docs/contribute/generate-ref-docs/contribute-upstream
+ https://kubernetes.io/docs/contribute/generate-ref-docs/quickstart
+ https://kubernetes.io/docs/contribute/generate-ref-docs/kubernetes-api
+ https://kubernetes.io/docs/contribute/generate-ref-docs/kubectl
+ https://kubernetes.io/docs/contribute/generate-ref-docs/kubernetes-components
+ https://kubernetes.io/docs/contribute/generate-ref-docs/prerequisites-ref-docs

### 高级贡献

+ https://kubernetes.io/docs/contribute/advanced

### 查看网站分析

+ https://kubernetes.io/docs/contribute/analytics

## 测试

+ https://kubernetes.io/docs/test




