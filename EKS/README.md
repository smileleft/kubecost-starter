# How to Deploy Kubecost on EKS

## Deploying Kubecost on an Amazon EKS cluster using Amazon EKS add-on - Prerequisites

```
Subscribe to Kubecost on AWS Marketplace
Install the following tools: kubectl, AWS CLI
Access to an EKS Cluster
```

## Enable Kubecost add-on using AWS CLI

```
aws eks create-addon \
  --addon-name kubecost_kubecost \
  --cluster-name $YOUR_CLUSTER_NAME \
  --region $AWS_REGION

# example output
{
  "addon": {
    "addonName": "kubecost_kubecost",
    "clusterName": "$YOUR_CLUSTER_NAME",
    "status": "CREATING",
    "addonVersion": "v1.97.0-eksbuild.1",
    "health": {
      "issues": []
    },
    "addonArn": "arn:aws:eks:$AWS_REGION:xxxxxxxxxxxx:addon/$YOUR_CLUSTER_NAME/kubecost_kubecost/90c23198-cdd3-b295-c410-xxxxxxxxxxxx",
    "createdAt": "2022-12-01T12:18:26.497000-08:00",
    "modifiedAt": "2022-12-01T12:50:52.222000-08:00",
    "tags": {}
  }
}
```
