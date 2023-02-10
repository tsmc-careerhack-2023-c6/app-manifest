# Application Manifest

## setup node taint

- create taint
```shell
kubectl taint nodes tsmc-vm-2-2 app=business1:NoSchedule
kubectl taint nodes tsmc-vm-2-3 app=business2:NoSchedule
kubectl taint nodes tsmc-vm-2-4 app=database:NoSchedule
kubectl taint nodes tsmc-vm-2-5 app=inventory:NoSchedule
```

- remove taint
```
kubectl taint nodes tsmc-vm-2-2 app=business1:NoSchedule-
kubectl taint nodes tsmc-vm-2-3 app=business2:NoSchedule-
kubectl taint nodes tsmc-vm-2-4 app=database:NoSchedule-
kubectl taint nodes tsmc-vm-2-5 app=inventory:NoSchedule-
```

## Production Environment Setup

- install
```shell
helm install careerhack .
```
- uninstall
```shell
helm uninstall careerhack
```

## Stage Environment Setup

- install
```shell
helm install -f values.stage.yaml careerhack .
```
- uninstall
```shell
helm uninstall careerhack
```
