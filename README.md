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

## Remove persistent volume

```
kubectl delete namespace kubecost
```

## Reference Resource

```
https://www.ibm.com/docs/en/kubecost/self-hosted/3.x?topic=SSW0JQG_3.0.x/install-and-configure/install/install.htm
https://nangman14.tistory.com/105
https://devocean.sk.com/blog/techBoardDetail.do?ID=164699&boardType=techBlog
```
