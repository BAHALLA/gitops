# k8s deployment

## nfs subdir external provisioner

 **NFS subdir external provisioner** is an automatic provisioner that use your existing and already configured NFS server to support dynamic provisioning of Kubernetes Persistent Volumes via Persistent Volume Claims [more details here](https://github.com/kubernetes-sigs/nfs-subdir-external-provisioner). 

NFS server in this deployment is configured as follows:
- IP : 192.168.1.9
- PATH: /srv/nfs/kubedata