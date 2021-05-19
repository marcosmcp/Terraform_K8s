## DESAFIO DEVOPS NATURA

## Instalação
```sh
terraform init no diretorio ./01_TERRAFORM EKS ON AWS
```
## Aplicando
```shs
terraform apply --auto-approve
```
## Adicionando o contexto do nosso cluster ao kubectl
```bash
aws eks --region us-east-1 update-kubeconfig --name k8s-desafio
```
```bash
kubectl get nodes
```
## Deploy o Ingress
```bash
kubectl apply -f 02_K8s/traefik/ingress.yml
```
## DEPLOY NGINX
* [desafio](https://github.com/marcosmcp/desafio)
```bash
kubectl apply -f 03_Helm/desafio.yml
```
## Get loadbalancer URL App
```bash
kubectl get all --all-namespaces
```

* Github: [@marcosmcp](https://github.com/marcosmcp)
* LinkedIn: [@marcosouzatech](https://linkedin.com/in/marcosouzatech)

