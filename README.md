   24  vi deployment.yaml 
   скопируй код из файла с этим же именем 
   вставить 
   shift+zz
   и так каждый раз когда будет новый файл 
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






1. **Edit Deployment File**: Open `deployment.yaml`, ensure it contains the correct configuration, then save and exit using `shift+zz` in vi.
    ```bash
    vi deployment.yaml
    ```

2. **Display Deployment Configuration**: Verify the contents of `deployment.yaml`.
    ```bash
    cat deployment.yaml
    ```

3. **Apply Deployment**: Execute the configuration to deploy.
    ```bash
    kubectl apply -f deployment.yaml
    ```

4. **List Deployments**: Check the active deployments to ensure yours is running.
    ```bash
    kubectl get deployments
    ```

5. **List Pods**: Ensure the pods related to your deployment are up and running.
    ```bash
    kubectl get pods
    ```

6. **Edit Nginx Service File**: Modify `nginx-service.yaml` as needed for your service configuration.
    ```bash
    vi nginx-service.yaml
    ```

7. **Apply Nginx Service**: Update your cluster with the Nginx service configuration.
    ```bash
    kubectl apply -f nginx-service.yaml
    ```

8. **Check Nginx Service Status**: Verify that the Nginx service is operational.
    ```bash
    kubectl get service nginx-service
    ```

9. **Review Nginx Service Configuration**: Look at the `nginx-service.yaml` file's current setup.
    ```bash
    cat nginx-service.yaml
    ```

10. **Access Nginx Service**: Navigate to the provided URL in your web browser to access the service.
    ```
    http://18.118.78.186:30001
    ```

11. **Delete Nginx Deployment**: Remove the Nginx deployment if necessary.
    ```bash
    kubectl delete deployment nginx-deployment
    ```

12. **Delete Nginx Service**: Similarly, remove the Nginx service if needed.
    ```bash
    kubectl delete service nginx-service
    ```

13. **Edit Postgres Deployment Configuration**: Adjust settings within `postgres-deployment.yaml` for the database.
    ```bash
    vi postgres-deployment.yaml
    ```

14. **Deploy Postgres Configuration**: Apply the changes for the Postgres deployment.
    ```bash
    kubectl apply -f postgres-deployment.yaml
    ```

15. **Verify Postgres Deployment**: Check that the Postgres deployment has been successfully applied.
    ```bash
    kubectl get deployments
    ```

16. **Check Postgres Pods**: Ensure the Postgres pods are functioning as expected.
    ```bash
    kubectl get pods
    ```

17. **Display Postgres Configuration**: Confirm the details of the Postgres deployment.
    ```bash
    cat postgres-deployment.yaml
    ```

18. **Edit Postgres Service File**: Update the `postgres-service.yaml` according to your service needs.
    ```bash
    vi postgres-service.yaml
    ```

19. **Apply Postgres Service**: Implement the new service settings.
    ```bash
    kubectl apply -f postgres-service.yaml
    ```

20. **List All Services**: Confirm all services, including Postgres, are correctly listed and active.
    ```bash
    kubectl get services
    ```

21. **Inspect Postgres Service Configuration**: Check the content of the `postgres-service.yaml`.
    ```bash
    cat postgres-service.yaml
    ```

22. **Modify Kanban App Deployment File**: Adjust `kanban-app-deployment.yaml` as needed for deployment.
    ```bash
    vi kanban-app-deployment.yaml
    ```

23. **Apply Kanban App Deployment**: Deploy the Kanban application changes.
    ```bash
    kubectl apply -f kanban-app-deployment.yaml
    ```

24. **Check Kanban App Deployments**: Verify the status and presence of the Kanban app deployments.
    ```bash
    kubectl get deployments
    ```

25. **Verify Kanban App Pods**: Ensure that the Kanban app's pods are live and running.
    ```bash
    kubectl get pods
    ```

26. **Review Kanban App Deployment File**: Peek into the `kanban-app-deployment.yaml` to verify its contents.
    ```bash
    cat kanban-app-deployment.yaml
    ```

27. **Adjust Kanban App Service Settings**: Edit `kanban-app-service.yaml` to align with your service specifications.
    ```bash
    vi kanban-app-service.yaml
    ```

28. **Deploy Kanban App Service Configuration**: Apply the Kanban app service modifications.
    ```bash
    kubectl apply -f kanban-app-service.yaml
    ```

29. **Navigate to Kanban App**: Open the Kanban app through the given URL in your browser.
    ```
    http://18.118.78.186:30000
    ```

30. **Review Kanban App Service File**: Check the details within the `kanban-app-service.yaml`.
    ```bash
    cat kanban-app-service.yaml
    ```

31. **Edit Kanban UI Deployment**: Update `kanban-ui-deployment.yaml` with the necessary UI configurations.
    ```bash
    vi kanban-ui-deployment.yaml
    ```

32. **Deploy Kanban UI**: Apply the UI deployment to the cluster.
    ```bash
    kubectl apply -f kanban-ui-deployment.yaml
    ```

33. **Inspect Kanban UI Deployments**: Ensure the Kanban UI has been deployed successfully.
    ```bash
    kubectl get deployments
    ```

34. **Verify Kanban UI Pods**: Check the status of the UI pods to confirm they are operational.
    ```bash
    kubectl get pods
    ```

35. **Display Kanban UI Deployment Configuration**: View the current setup in `kanban-ui-deployment.yaml`.
    ```bash
    cat kanban-ui-deployment.yaml
    ```

36. **Adjust Kanban UI Service Settings**: Make necessary changes to `kanban-ui-service.yaml`.
    ```bash
    vi kanban-ui-service.yaml
    ```

37. **Apply Kanban UI Service Configuration**: Update the cluster with the new UI service settings.
    ```bash
    kubectl apply -f kanban-ui-service.yaml
    ```

38. **List All Current Services**: Check all running services to ensure the UI service is active.
    ```bash
    kubectl get services
    ```

39. **Access Kanban UI in Browser**: Open the provided URL to view the Kanban UI.
    ```
    http://18.118.78.186:30001
    ```

40. **Review Kanban UI Service Configuration**: Examine the details in the `kanban-ui-service.yaml`.
    ```bash
    cat kanban-ui-service.yaml
    ```

41. **View Command History**: Retrieve the list of executed commands for review or documentation purposes.
    ```bash
    history
    ```

