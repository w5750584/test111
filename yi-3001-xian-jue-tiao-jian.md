#### 作为目前最火的容器编排工具k8s。在安装过程中存在不少啃，为了大家少采坑，我把自己的安装过程记录下来本文以二进制文件方式从头安装k8s，以便让大家能测底了解k8s各组件的关系。

#### 下面是k8s需要的组件介绍：



* ##### 必备组件：

```
etcd
```

* ##### 集群所有机器组件：

```
flannled
```

* ##### master组件：

```
kubectl
kube-apiserver
kube-scheduler
kube-controller-manager
```

* ##### node组件：

```
docker
kubelet
kub-proxy
```



#### 本文以俩台机器为例：

```
master 192.168.61.128
node 192.168.61.129
etcd1 192.168.1.128
etcd2 192.168.1.129
```





