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

Show DIFF
Sinc only one component
Show new ReplicaSet
Switch to network flow
show pop-up versions


Resume deployment usin UI


#CLI Plugin
Show rollout status using CLI
```
kubectl argo rollouts get rollout bluegreen-demo
```

Promote deployment using CLI
```
kubectl argo rollouts promote bluegreen-demo
```

##Roll back
Show images gui and cli


##HELM

helm upgrade --install bluegreen-demo  --namespace bluegreen-demo  -f helm/values/prd/values.yaml helm/demo
helm upgrade --install bluegreen-demo-tst  --namespace bluegreen-demo-tst -f helm/values/tst/values.yaml helm/demo
helm upgrade --install bluegreen-demo-acc  --namespace bluegreen-demo-acc -f helm/values/acc/values.yaml helm/demo


