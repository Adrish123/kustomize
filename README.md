
If Using kubectl Built-in Kustomize

kubectl version --client
```
Steps to install Kustomize tool in linux

curl -s "https://raw.githubusercontent.com/kubernetes-sigs/kustomize/master/hack/install_kustomize.sh" | bash
sudo mv kustomize /usr/local/bin/

```
cd manifest
```
kubectl apply -f .\namespace.yaml
```
cd manifest\ind\blue
```
kubectl apply -f .\deployment.yaml
```
cd ..

cd overlays\dev
```
kubectl apply -k .
```

![image](https://github.com/user-attachments/assets/ccb91248-d266-4bd4-9acd-4d934f0d0e56)
