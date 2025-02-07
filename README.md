
If Using kubectl Built-in Kustomize
```
kubectl version --client
```
Steps to install Kustomize tool in linux
```
curl -s "https://raw.githubusercontent.com/kubernetes-sigs/kustomize/master/hack/install_kustomize.sh" | bash
sudo mv kustomize /usr/local/bin/
```

Create Namespace:
```
cd manifest
kubectl apply -f .\namespace.yaml
```

Deploy Nginx app:
```
cd manifest\ind\blue
kubectl apply -f .\deployment.yaml
```

Run Kuztomization: 
```
cd ..\overlays\dev
kubectl apply -k .
```

Verify results to check if the resource limits have been modified in the deployment:
```
kubectl describe deployment nginx-app -n my-ns
```
