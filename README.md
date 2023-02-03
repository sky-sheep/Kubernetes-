# Kubernetes
k8s离线一键部署（centos7.9）

创建/k8s文件夹，解压到/k8s文件夹下

```shell
# 设置节点名称 不同节点设置不同名称
hostnamectl set-hostname k8s-01

#授权限
chmod +x k8s.sh

#主节点启动命令
./k8s.sh --master-address 192.168.0.200 --node-type master
#子节点启动命令
./k8s.sh --master-address 192.168.0.200 --node-type node

```
