# knawd operator

Work In Progress

Currently working on 

1. [custom service accounts](https://sdk.operatorframework.io/docs/advanced-topics/multi-sa/)

2. Knative patch 
    ```
    kubectl patch configmap/config-features -n knative-serving --type merge --patch '{"data":{"kubernetes.podspec-runtimeclassname":"enabled"}}'
    ```

## build

See https://sdk.operatorframework.io/docs/building-operators/ansible/tutorial/

```
make docker-build docker-push

make bundle bundle-build bundle-push
```

