---
date: 2020-09-30T11:25
---

# kubernetes-tips

Tricks on K8S cluster upgrades:


```
kubectl get pod --all-namespaces | egrep -i 'Invalid|Error|Crash|Failed|Unknown|Pending'
```

