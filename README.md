kubectl apply -f deployment/rest-app.yml -o yaml >> rest-app.yml
kubectl apply -f deployment/mysql-app.yml -o yaml >> mysql-app.yml

port forwarding for rest
kubectl port-forward rest-deployment-5b65996c95-nbmq4 8080:8080 
OR
minikube service rest-service --url

enable ingress to show ipv4 address
minikube addons enable ingress
minikube tunner -> enable ingress resources available at localhost
>minikube addons enable ingress  -> enable ingress

after creating ingress map the value in etc/hosts 
OR
C:\Windows\System32\drivers\etc\hosts  -> in windows