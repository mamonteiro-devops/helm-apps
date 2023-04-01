
helm repo add grafana https://grafana.github.io/helm-charts


helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

helm repo update


helm install prom-graf prometheus-community/kube-prometheus-stack --namespace monitoring --create-namespace --values values.yaml

helm install prom-graf grafana/grafana --namespace monitoring --create-namespace --values values.yaml

