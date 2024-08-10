# How to deploy rabbitmq queues in k8s

- Deploy rabbitmq operator using helm

```
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install my-release bitnami/rabbitmq-cluster-operator
```
- Create a cluster.yaml definition file following format given in `example-cluster.yaml` file and run :

```
kubectl apply -f cluster.yaml -n <namespace>
```