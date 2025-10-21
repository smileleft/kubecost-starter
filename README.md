# kubecost-starter
how to start kubecost

## Install kubecost via Helm

```
helm install kubecost \
  --repo https://kubecost.github.io/kubecost kubecost \
  --namespace kubecost --create-namespace \
  --set global.clusterId=someclustername
```
