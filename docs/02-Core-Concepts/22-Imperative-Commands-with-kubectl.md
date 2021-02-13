# Certification Tips - Imperative Commands with kubectl
  - Take me to the [Tutorial](https://kodekloud.com/courses/539883/lectures/10503265)

# Imperative Commands
# Create Objects
kubectl run --image=nginx nginx

kubectl create deployment --image=nginx nginx

kubectl exposse deployment nginx --port 80

# Update Objects
kubectl  edit deployment nginx

kubectl  scale deployment nginx --replicas=5

kubectl set image deployment nginx nginx=nginx:1.18

# Imperative Object Configuration Files
kubectl create -f nginx.yaml

kubectl replace -f nginx.yaml

Kubectl replace --force -f nginx.yaml

kubectl delete -f nginx.yaml

# Better to first replace the config file rather than edit 

## Declarative

kubectl apply -f nginx.yaml

kubectl apply -f /path/to/config-files
