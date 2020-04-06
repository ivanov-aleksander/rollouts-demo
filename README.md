##Add application CRD

```bash
kubectl create -f argo-cd/application.yaml
```

AutoSync is disabled as a result applications status is OutOfSync. 
Check DIFF in UI

Show deploied resources in namespace
```
kubectl get all
```

Sync
Show helth statuses
show resources
show logs for pods
show events for pods

Show trafic flow (Network)

##Update image tag

