# kubecost-starter
how to start kubecost

## Install kubecost via Helm

```
helm install kubecost \
  --repo https://kubecost.github.io/kubecost kubecost \
  --namespace kubecost --create-namespace \
  --set global.clusterId=someclustername
```

## Add Helm Repository first and Sacn for updates

```
helm repo add kubecost https://kubecost.github.io/kubecost/
helm repo update
helm install kubecost kubecost/kubecost -n kubecost --create-namespace
```

## Uninstall

```
helm uninstall kubecost -n kubecost
```
