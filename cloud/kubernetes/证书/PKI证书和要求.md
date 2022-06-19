# PKI证书和要求

PKI证书用于TLS认证。


## 集群如何使用证书


Client certificates         for the kubelet    to authenticate to the API server
Kubelet server certificates for the API server to talk to the kubelets
Client certificates         for the API server to talk to the kubelets





+ API服务器对kubelet进行认证的客户端证书
+ API服务器与kubelet进行通信的kubelet服务器证书
+ API服务器端点的服务器证书
+ API服务器对集群管理员进行认证的客户端证书
+ API服务器与kubelet进行通信的客户端证书
+ API服务器与etcd进行通信的客户端证书
+ 控制器管理器与API服务器进行通信的客户端证书或kubeconfig
+ 调度器与API服务器进行通信的客户端证书或kubeconfig
+ 前端代理的客户端和服务端证书












## 证书的存放位置

使用kubeadm安装Kubernetes时，大多数证书存放在/etc/kubernetes/pki中，用户账号证书在/etc/kubernetes中。

## 手动配置证书


### 



### 



### 












## 为用户帐号配置证书





































## 参考文档

+ https://kubernetes.io/docs/setup/best-practices/certificates




