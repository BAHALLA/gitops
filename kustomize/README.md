# k8s deployments

## Infra deployments

### Nfs subdir external provisioner

 **NFS subdir external provisioner** is an automatic provisioner that use your existing and already configured NFS server to support dynamic provisioning of Kubernetes Persistent Volumes via Persistent Volume Claims [more details here](https://github.com/kubernetes-sigs/nfs-subdir-external-provisioner). 
NFS server in this deployment is configured as follows:
- IP : 192.168.1.9
- PATH: /srv/nfs/kubedata

### Strimzi

[Strimzi](https://strimzi.io/) is a k8s operator to deploy and manage apache kafka, it provide cluster setup, topic management, users and more. 
This setup is based on [strimzi doc](https://strimzi.io/docs/operators/latest/deploying.html#deploy-prereqs-str) and strimzi [github repository](https://github.com/strimzi/strimzi-kafka-operator)

### Kube-prometheus-stack

[Kube-prometheus-stack](https://github.com/prometheus-operator/kube-prometheus) is a collection of Kubernetes manifests, Grafana dashboards, and Prometheus rules combined with documentation and scripts to provide easy to operate end-to-end Kubernetes cluster monitoring with Prometheus using the Prometheus Operator. 
deployed using kustomize and [community helm chart](https://github.com/prometheus-community/helm-charts/tree/main/charts/kube-prometheus-stack)

### Nginx ingress controller

[Nginx ingress controller](https://docs.nginx.com/nginx-ingress-controller/intro/overview/) is an implementation of a Kubernetes [Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/) Controller for NGINX.
deployed using [Installation with Manifests](https://docs.nginx.com/nginx-ingress-controller/installation/installation-with-manifests/) 




