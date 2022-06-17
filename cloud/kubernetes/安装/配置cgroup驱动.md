# 配置cgroup驱动

kubelet的cgroup驱动必须匹配容器运行时的cgroup驱动。

## 配置容器运行时的cgroup驱动

kubeadm会把kubelet当做systemd服务来管理，在基于kubeadm的安装中，推荐使用systemd驱动，而非cgroupfs驱动。

## 配置kubelet的cgroup驱动

执行kubeadm init时，可以传递KubeletConfiguration。

KubeletConfiguration的cgroupDriver字段用于控制kubelet的cgroup驱动。

在v1.22中，如果没有设置KubeletConfiguration的cgroupDriver字段，kubeadm会把它默认成systemd。

kubeadm对集群中的所有节点都使用相同的KubeletConfiguration。

KubeletConfiguration存放在kube-system命名空间的ConfigMap中。

执行init、join和upgrade子命令时，kubeadm会把KubeletConfiguration写入到/var/lib/kubelet/config.yaml文件中，并传递给节点的kubelet。

配置KubeletConfiguration的cgroupDriver字段：

```
# kubeadm-config.yaml
kind: ClusterConfiguration
apiVersion: kubeadm.k8s.io/v1beta3
kubernetesVersion: v1.21.0
---
kind: KubeletConfiguration
apiVersion: kubelet.config.k8s.io/v1beta1
cgroupDriver: systemd
```

执行kubeadm init命令：

```
kubeadm init --config kubeadm-config.yaml
```

## 修改cgroup驱动

### 修改kubelet的ConfigMap

+ 编辑kubelet-config：`kubectl edit cm kubelet-config -n kube-system`

+ 在ConfigMap的kubelet:中添加或修改cgroupDriver字段：`cgroupDriver: systemd 或 cgroupfs`

### 修改节点的cgroup驱动

一次一个节点，在集群的每个节点中执行：
+ 隔离节点：`kubectl drain <node-name> --ignore-daemonsets`
+ 停止kubelet：`systemctl stop kubelet`
+ 停止容器运行时
+ 修改容器运行时的cgroup驱动：`systemd 或 cgroupfs`
+ 设置/var/lib/kubelet/config.yaml：`cgroupDriver: systemd 或 cgroupfs`
+ 启动容器运行时
+ 启动kubelet：`systemctl start kubelet`
+ 解除节点隔离：`kubectl uncordon <node-name>`
+ 确认节点和工作负载的健康状况

## 修改cgroup驱动：替换节点

+ 修改kubelet的ConfigMap
+ 添加新节点
+ 确认工作负载是否迁移到新节点
+ 删除旧节点

## 参考文档

+ https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/configure-cgroup-driver




