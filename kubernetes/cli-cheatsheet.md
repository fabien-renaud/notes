[Go back to Kubernetes](https://github.com/fabien-renaud/notes/blob/master/kubernetes)

# Kubernetes - CLI Cheatsheet ☄️

#### Apply manifest
```sh
cmd   kubectl apply -f <manifest.yaml>
```

#### Get status of resources
```sh
cmd   kubectl get <pods|deployments|services|ingress>
```

#### Get resources consumption
```sh
cmd   kubectl top <pod|service>
```

#### Get resource logs
```sh
cmd   kubectl logs <resource-name>
```

#### Change namespace
```sh
cmd   kubectl config set-context --current --namespace=<namespace-name>
```

#### Forward port
```sh
cmd   kubectl port-forward pod/<pod-name> <listening-port>:<forwarding-port>
```

## That's all !
*Don't forget to give a* ⭐️ *if this markdown helped you !*
