# homelab-master
Master repo for building, configuring and deploying the infrastructure to the Homelab! The goal will be to automate the entire process while also trying to implement best practices and be cloud agnostic.

`*-forge` - Terraform repos

`*-ignite` - Ansible repos

`*-launch` - Helm wrapper repos

## To do
- [x] Create a list of desired Homelab services and their purpose
- [x] Terraform to deploy VMs
- [x] Ansible to configure and install K3s
- [x] Ansible to configure and install rook-ceph
- [x] Upgrade to Proxmox 9
- [x] Determine how to handle secrets (storing, push) and passwords
- [x] Determine Deployment strategy (Bootstrap vs ArgoCD): ArgoCD
- [ ] Refactor the cp-deply project to use ArgoCD app of apps to bootstrap the following services:
  - [ ] MetalLB
  - [ ] Ingress-nginx
  - [ ] Cert-manager
  - [ ] External-secrets
  - [ ] Infisical
  - [ ] Bitwarden
  - [ ] Rook-Ceph
  - [ ] CNPG
  - [ ] Keycloak
  - [ ] Gitea
  - [ ] Nexus
  - [ ] Argocd
  - [ ] K8s dashboard
  - [ ] Paperless
  - [ ] Plex

**UPDATE:** We got a task Board! [HERE!](https://github.com/users/pukar10/projects/1)

## Index

[Proxmox-forge](https://github.com/pukar10/proxmox-deploy)
* Declarative Terraform repo to deploy n VMs onto n hosts with differing configurations.

[k3-ignite](https://github.com/pukar10/k3-automation)
* Declarative ansible repo to configure VMs installing the following
  *  Minimal k3s
  *  Containerd as CRI
  *  Flannel as CNI
*  Optional playbooks to install
  *  MetalLB to replace serviceLB
  *  Ingress-nginx to replace traefik
  *  Rook-ceph as a storage solution

[cert-manager-launch](https://github.com/pukar10/cert-manager-launch)
* Automates getting/renewing certs

external-secrets-launch (tba)
* Able to generates secret and push to secret-store or pull secrets from secret-store and save as a secret for apps to consume.

infisical-launch (tba)
* Secret store

bitwarden-launch (tba)
* Password manager

[cloudnativepg-launch](https://github.com/pukar10/cloudnativepg-launch)
* Operator to manage one or more Postgres clusters

[keycloak-launch](https://github.com/pukar10/keycloak-launch)
* SSO

gitea-launch (tba)
* Code repository

