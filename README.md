#### 1、服务器要求：

\*  系统版本：centos7.4

\*  网络环境：所有节点可以互通

\*  注意事项：关闭集群所有服务器selinux，iptables

#### 2、软件依赖：

##### \*  必备服务，可以安装到master或者node上，或者其他机器也可以：

```
etcd
```

##### \*  集群所有服务器：

```
flanneld
```

##### \*  master：

```
kubectl
kube-apiserver
kube-scheduler
kube-controller-manager
```

##### \*  node：

```
docker
kubelet
kub-proxy
```

#### 3、在集群所有服务器/etc/hosts添加一下内容：

```
master 192.168.61.128
node1 192.168.61.129
etcd1 192.168.1.128
etcd2 192.168.1.129
```



