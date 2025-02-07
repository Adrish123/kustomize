
If Using kubectl Built-in Kustomize

kubectl version --client
```
Steps to install Kustomize tool in linux

curl -s "https://raw.githubusercontent.com/kubernetes-sigs/kustomize/master/hack/install_kustomize.sh" | bash
sudo mv kustomize /usr/local/bin/

```
cd manifest
kubectl apply -f .\namespace.yaml
```
cd manifest\ind\blue
kubectl apply -f .\deployment.yaml
```
cd ..
cd overlays\dev
kubectl apply -k .
```

![image](https://github.com/user-attachments/assets/0c4de4dc-832d-4f39-90b1-3f1fc09dc463)
