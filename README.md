   24  vi deployment.yaml 
   25  cat deployment.yaml 
   26  kubectl apply -f deployment.yaml
   27  kubectl get deployments
   28  kubectl get pods
   31  vi nginx-service.yaml
   32  kubectl apply -f nginx-service.yaml
   33  kubectl get service nginx-service
   34  cat nginx-service.yaml 
   36  http://18.118.78.186:30001 in browser
   37  kubectl delete deployment nginx-deployment
   38  kubectl delete service nginx-service
   39  vi postgres-deployment.yaml
   40  kubectl apply -f postgres-deployment.yaml
   41  kubectl get deployments
   42  kubectl get pods
   43  cat postgres-deployment.yaml 
   44  vi postgres-service.yaml
   45  kubectl apply -f postgres-service.yaml
   46  kubectl get services
   47  cat postgres-service.yaml 
   48  vi kanban-app-deployment.yaml
   49  kubectl apply -f kanban-app-deployment.yaml
   50  kubectl get deployments
   51  kubectl get pods
   52  cat kanban-app-deployment.yaml 
   53  vi kanban-app-service.yaml
   54  kubectl apply -f kanban-app-service.yaml
   55  kubectl get services
   57  http://18.118.78.186:30000 in your browser
   58  cat kanban-app-service.yaml 
   59  vi kanban-ui-deployment.yaml
   60  kubectl apply -f kanban-ui-deployment.yaml
   61  kubectl get deployments
   62  kubectl get pods
   63  cat kanban-ui-deployment.yaml 
   64  vi kanban-ui-service.yaml
   65  kubectl apply -f kanban-ui-service.yaml
   66  kubectl get services
   67  http://18.118.78.186:30001  in browser
   68  cat kanban-ui-service.yaml 
   69  history
[ec2-user@ip-172-31-20-136 ~]$ 