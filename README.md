# kubernetes

### Rodar o arquivo de configuração do kubernete

```sh
kubectl create -f dev-config.yml
kubectl create -f pod-mysql.yml
kubectl create -f pod-service-nginx.yml
```
### Lista de serviços disponível.

```sh
kubectl get pods
```
### Lista de ips dos serviços 

```sh
kubectl get -w svc 
```
### Acessar ssh o serviço

```sh
kubectl exec --stdin --tty servico-nginx -- /bin/bash
```
### Install telenet

```sh
apt-get update && apt-get install telnet
telnet [ip da lista de serviços] [3306]


```sh
Trying 10.105.142.55...
Connected to 10.105.142.55.
Escape charac```ter is '^]'.
J
```

### Variáveis de ambiente
MYSQL_ROOT_PASSWORD: q1w2e3r4
MYSQL_DATABASE: empresa
MYSQL_PASSWORD: q1w2e3r4
