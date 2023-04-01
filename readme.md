

k create ns cloudflow
helm install strimzi strimzi/strimzi-kafka-operator --namespace cloudflow

helm delete strimzi -n cloudflow


helm ls -n cloudflow


#review this file
https://www.civo.com/learn/installing-an-apache-kafka-cluster-on-kubernetes-using-strimzi-and-gitops
