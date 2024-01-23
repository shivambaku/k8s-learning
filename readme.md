#### Notes

* Deleting the pod will auto restart it because it try to reach the desired state.
* Environment variables only reset when the pod is restarted.
* Vercel (Frontend), Kubernetes (Backend), Managed PSQL
* Resource limit solves the issue of k8s trying to add another pod when the node cannot handle anymore.
* Good rule of thumb
    * Set memory requests ~10% higher than the average memory usage of your pods
    * Set CPU requests to 50% of the average CPU usage of your pods
    * Set memory limits ~100% higher than the average memory usage of your pods
    * Set CPU limits ~100% higher than the average CPU usage of your pods


#### Useful commands

```kubectl apply -f CONFIG```

```kubectl proxy```

```kubectl get pods```

```kubectl delete pods POD```

```kubectl get svc```

```kubectl get configmaps```

```kubectl get hpa```


