Install Nginx Ingress Controller

$ kubectl apply -f https://kind.sigs.k8s.io/examples/ingress/deploy-ingress-nginx.yaml

$ kubectl get ns


Can see new ns "ingress-nginx"

Create the application using deployment.yml

$ kubectl apply -f app1.yml -f app2.yml 

$ kubectl get pods

$ kubectl get svc

Create ingress using ingress.yml


Apply the ingress:

$  kubectl apply -f ingress.yml 

Get the ingress IP:

$ kubectl get ingress

Check controller logs:

$ kubectl logs -n ingress-nginx deploy/ingress-nginx-controller

Verify endpoints:

$ kubectl get endpoints app1-svc app2-svc


![4B15AC57-2775-4BC5-B679-5E74B0518E0E](https://github.com/user-attachments/assets/d9c208f1-6e0e-404f-8963-67897f0eda29)




