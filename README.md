# kubernetes-deployment
sudo -i
kubectl get nodes
kubectl  create  deployment  <Deplyment-Name>  --image=<Container-Image> kubectl  create  deployment  my-first-deployment  -- image=stacksimplify/kubenginx:1.0.0
kubectl get po
 kubectl get rs(replicat create and pod create deployment chesthe)
  scalling 
 kubectl  scale  --replicas=5  deployment/my-first-deployment
kubectl get po
  expose
  kubectl  expose  deployment  my-first-deployment  --type=LoadBalancer  -- port=80  --target-port=80  --name=my-first-deployment-service
kubectl svc(already exits)
  
  a1cf to .com:80 google search
  
  
  
  update deployment
  rollout
  
kubectl set image  deployment/my-first-deployment kubenginx=stacksimplify/kubenginx:2.0.0 --record=true
  rollout
   kubectl  rollout status deployment/my-first-deployment
  refresh version 2
  kubectl set image deployment/my-first-deployment kubenginx=stack simplify/kubenginx:3.0.0 --record=true
  kubectl rollout history deployment/my-first-deployment deployment.apps/my-first-deployment
  kubectl set image  deployment/my-first-deployment kubenginx=stacksimplify/kubenginx:4.0.0 --record=true
  kubectl set image  deployment/my-first-deployment kubenginx=stacksimplify/kubenginx:1.0.0 --record=true
kubectl rollout undo deployment/my-first-deployment --to-revision=3
kubectl rollout undo deployment/my-first-deployment --to-revision=6
kubectl rollout undo deployment/my-first-deployment --to-revision=6
kubectl set resources deployment/my-first-deployment -c=kubenginx --limits=cpu=20m,memory=30mi
kubectl describe deployment my-first-deployment
  kubectl -d -t eks cluster kubernetes deployment
 
 
  
  
