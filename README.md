### Kubernetes,

**Getting started ,** https://kubernetes.io/docs/setup/

**Install Tools ,** https://kubernetes.io/docs/tasks/tools/

**Installing Kubernetes with deployment tools ,** https://kubernetes.io/docs/setup/production-environment/tools/

<br>

### KUBEADM,

**Bootstrapping clusters with kubeadm ,** https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/

**Installing kubeadm ,** https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/install-kubeadm/

<br>

### System configuration,

**Keep firewalld and SELinux turned off,**

`[anup@rhel-92-04 ~]$ sudo systemctl status firewalld.service `

`[anup@rhel-92-04 ~]$ sudo systemctl stop firewalld.service `

`[anup@rhel-92-04 ~]$ sudo systemctl disable firewalld.service`
 

`[anup@rhel-92-04 ~]$ sudo setenforce 0`

<br>

**For : [WARNING Swap]: swap is enabled; production deployments should disable swap unless testing the NodeSwap feature gate of the kubelet**

`[anup@rhel-92-04 ~]$ sudo swapoff -a`

<br>

### Troubleshoot

`[anup@rhel-92-04 ~]$ sudo kubeadm reset`

`[anup@rhel-92-04 ~]$ ls -ltra`

<br>
