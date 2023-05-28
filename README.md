# O projeto helm-chart consiste em provisionar deployment, service e hpa em seu cluster kubernetes

### Clone o repositório:
```bash
git clone https://github.com/deividduarte20/helm-chart.git
```

### Entre no diretório:
```bash
cd helm-chart
```

### Altere o arquivo de values.yaml conforme sua necessida exemplo namespace.

### Caso queria simular sem executar a instalação do chart
```bash
helm install app --debug --dry-run ./helm-chart/
```

### Instalar chart:
```bash
helm install app ./helm-chart/
```

### Para consultar:
```bash
kubectl get all -n seu-namespace
```

### Para desinstalar o chart
```bash
helm uninstall app
```
