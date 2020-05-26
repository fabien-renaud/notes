# Kubernetes - CLI Cheatsheet ☄️

#### Apply manifest
```sh
cmd   kubectl apply -f manifest.yaml
```

#### Get status of resources
```sh
cmd   kubectl get [pods|deployments|services|ingress]
```

#### Get resources consumption
```sh
cmd   kubectl top [pod|service]
```

#### Get resource logs
```sh
cmd   kubectl logs resourceName
```

#### Forward port
```sh
cmd   kubectl port-forward pod/podname listeningPort:forwardingPort
```

## That's all !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
