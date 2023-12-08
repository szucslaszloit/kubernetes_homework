Installation, deployment commands:

kubectl apply -f frontapp-deployment.yaml

kubectl apply -f frontapp-service.yaml

kubectl apply -f frontapp-ingress.yaml

kubectl apply -f backapp-deployment.yaml

kubectl apply -f backapp-service.yaml


kubectl logs, frontapp, backapp:

kubectl logs backapp-7df99c4c58-6824f
kubectl logs frontapp-64d9776bf-65m2f

Command for listing all frontapp related resources:

kubectl get all -l homework=frontapp

Commands for deleting both applications and resources:

kubectl delete all -l training=block
kubectl delete ingress frontapp



