# Application Manifest

## Production Environment Setup

- install
```shell
helm install careerhack .
```
- uninstall
```shell
helm uninstall careerhack .
```

## Stage Environment Setup

- install
```shell
helm install -f values.stage.yaml careerhack .
```
- uninstall
```shell
helm uninstall careerhack .
```
