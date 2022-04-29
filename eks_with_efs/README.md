  **INSTALL aws efs-ecs driver** 
  
  
  **create EKS cluster**

     cat cluster.yaml

     eksctl create cluster -f cluster.yaml


  **create ConfigMap | StorageClass | PersistentVolume | PersistentVolumeClaim | Deployment**
  
     cat pg-deployment.yaml
     kubectl apply -f pg-deployment.yaml
     

