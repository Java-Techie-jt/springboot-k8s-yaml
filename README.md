# springboot-k8s-yaml

1. Run spring boot app in docker \
```docker build -t springboot-k8-example:1.1 . ```    
2. Create/update deployment \
``` kubectl apply -f deployment.yaml```
3. check the deployment \
```kubectl get deployments```
4. check the pods \
``` kubectl get pods```
5. Get deployment logs \
``` kubectl logs deployment/spring-boot-k8s```
6. Get pod log \
```kubectl logs <POD-NAME>```
7. run service file \
``` kubectl apply -f .\service.yaml```
8. Get all the service \
```kubectl get svc```
9. access the link using \
   NodeInternalIP:<NODE-PORT>


Reference: 
1. https://stackoverflow.com/questions/60518658/how-to-get-logs-of-deployment-from-kubernetes
2. 