# kube-loki


A Loki-based logging stack consists of 3 components:

promtail is the agent, responsible for gathering logs and sending them to Loki.
loki is the main server, responsible for storing logs and processing queries.
Grafana for querying and displaying the logs.


Install loki stack using that command:
```
helm install loki grafana/loki-stack --values loki-stack.yaml -n monitoring
```
to uninstall stack:
```
helm uninstall loki -n monitoring
```
make sure you have added the data source configuration for loki in grafana configmap. 