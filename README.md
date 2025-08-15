# homelab-master
Master repo for deploying the infrastructure to my Homelab

## To do
- [x] Upgrade to Proxmox 9
- [ ] Determine how to handle secrets (storing, push)
- [ ] Create a list of desired Homelab services
- [ ] Finish all infrastrcuture deploy repos

## Index

Cert-manager-deploy

External-secrets-deploy
* Can both pull and generate secrets. Able to push them to a secret store.



[Proxmox-deploy](https://github.com/pukar10/proxmox-deploy)
* Declarative Terraform repo to deploy n VMs onto n hosts with differing configurations.

[k3-automation](https://github.com/pukar10/k3-automation)
* Declarative ansible repo to configure VMs installing the following
  *  Minimal k3s replacing servicelb with metallb and traefik with ingress-nginx
  *  Containerd as CRI
  *  Flannel as CNI
  *  Rook-ceph as storage solution

CloudnativePG-deploy

Keycloak-deploy

