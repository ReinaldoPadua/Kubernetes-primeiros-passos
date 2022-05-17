## Namespace

```
kubectl get namespace

kubectl get namespace kube-system

kubectl get namespace kube-system -o=YAML

kubectl get namespace kube-system -o=JSON

kubectl apply -f '.\1 - namespace.yaml'

```

## POD

```
kubectl get pod -n kube-system

kubectl describe pod coredns-d76bd69b-jpj4x -n kube-system

kubectl logs coredns-d76bd69b-jpj4x -n kube-system

kubectl get pod -n desenvolvimento-frontend
```

## ConfigMap

```
kubectl get configmap -n desenvolvimento-frontend

kubectl delete configmap frontend-configmap -n desenvolvimento-frontend

```

## Deployment

```
kubectl apply -f '.\2 - deployment.yaml'

kubectl get deployment -n desenvolvimento-frontend

kubectl delete deployment frontend-deployment  -n desenvolvimento-frontend

```

## Autoscaling

```
kubectl get HorizontalPodAutoscaler -n desenvolvimento-frontend

kubectl delete HorizontalPodAutoscaler frontend-autoscaling -n desenvolvimento-frontend
```

## Service

```
kubectl apply -f '.\3 - service.yaml'

kubectl get service -n desenvolvimento-frontend

kubectl delete service frontend-service  -n desenvolvimento-frontend

```

## Ingress

```
kubectl apply -f '.\4 - ingress.yaml'

kubectl get ingress -n desenvolvimento-frontend

kubectl delete ingress frontend-ingress  -n desenvolvimento-frontend

```
