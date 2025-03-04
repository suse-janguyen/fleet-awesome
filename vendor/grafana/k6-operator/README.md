docs -- 
https://grafana.com/docs/k6/latest/set-up/set-up-distributed-k6/install-k6-operator/

helm steps 

helm repo add grafana https://grafana.github.io/helm-charts
helm repo update
helm install k6-operator grafana/k6-operator

turn test.js files into ConfigMap, refrenced by TestRun CRD.

