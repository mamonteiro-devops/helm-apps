

k create ns cloudflow
helm install strimzi strimzi/strimzi-kafka-operator --namespace cloudflow

helm delete strimzi -n cloudflow


helm ls -n cloudflow


### review this file
https://www.civo.com/learn/installing-an-apache-kafka-cluster-on-kubernetes-using-strimzi-and-gitops

### build the helm chart for strimzi cluster
```bash
--(NOT RUN ANOTHER TIME)
helm create strimzi-cluster
```

For example, to roll back the Helm chart named deployed-mdm to version 1, run the following command:
```
helm history <release-name> -n <namespace>
helm rollback <release-name> <revision number> -n <namespace>
helm history <release-name> -n <namespace>
helm template strimzi-cluster strimzi-cluster 
```


[cp-helm-charts](cp-helm-charts)

k create ns confluent
helm install cp-helm-charts ./cp-helm-charts -n confluent

helm delete cp-helm-charts -n confluent


[confluent-for-kubernetes](confluent-for-kubernetes)
