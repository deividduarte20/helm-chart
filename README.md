# O projeto helm-chart consiste em provisionar deployment, service e hpa em seu cluster kubernetes

### Clone o repositório:
```bash
git clone https://github.com/deividduarte20/helm-chart.git
```

### Entre no diretório:
```bash
cd helm-chart
```

## Criar namespace
```bash
kubectl create ns <nome-namespace>
```

### Caso queria simular sem executar a instalação do chart
```bash
helm install app --debug --dry-run ./helm-chart/ -n <nome-namespace>
```

### Instalar chart:
```bash
helm install app ./helm-chart/ -n seu-namespace
```

### Para consultar recursos no cluster:
```bash
kubectl get all -n seu-namespace
```
### Para consultar release helm:
```bash
helm list -n seu-namespace
```

### Para desinstalar o chart
```bash
helm uninstall app -n seu-namespace
```
