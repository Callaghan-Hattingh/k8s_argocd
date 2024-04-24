# argocd_bootstrap

Requirements:
* minikube
* Argocd-autopilot cli tool
* kubectl
* k9s

create minikube cluster:
```shell
minikube start
```
set envs below:
```shell
export GIT_TOKEN=...
export GIT_REPO=https://github.com/Callaghan-Hattingh/k8s_argocd.git
```
setup argo on cluster 
```shell
argocd-autopilot repo bootstrap --recover
```