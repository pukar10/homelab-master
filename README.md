# homelab-master
Master repo for deploying the infrastructure to my Homelab

## To do
- [x] Upgrade to Proxmox 9
- [ ] Determine how to handle secrets (storing, push) and passwords
- [ ] Create a list of desired Homelab services and their purpose
- [ ] Finish all infrastrcuture deploy repos
- [ ] Finish all service deploy repos

## Index

[Proxmox-deploy](https://github.com/pukar10/proxmox-deploy)
* Declarative Terraform repo to deploy n VMs onto n hosts with differing configurations.

[k3-automation](https://github.com/pukar10/k3-automation)
* Declarative ansible repo to configure VMs installing the following
  *  Minimal k3s replacing servicelb with metallb and traefik with ingress-nginx
  *  Containerd as CRI
  *  Flannel as CNI
  *  Rook-ceph as storage solution

Cert-manager-deploy
* Automates getting/renewing certs

External-secrets-deploy
* Able to generates secret and push to secret-store or pull secrets from secret-store and save as a secret for apps to consume.

Infisical-deploy
* Secret store

Bitwarden
* Password manager

CloudnativePG-deploy
* Operator to manage one or more Postgres clusters

Keycloak-deploy
* SSO

Gitea
* Code repository


