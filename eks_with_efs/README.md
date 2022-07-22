 

- Install Kubectl
  apt-get update
  curl -o kubectl https://amazon-eks.s3-us-west-2.amazonaws.com/1.21.2/2021-07-05/bin/linux/amd64/kubectl
  openssl sha1 -sha256 kubectl
  chmod +x ./kubectl
  mkdir -p $HOME/bin && cp ./kubectl $HOME/bin/kubectl && export PATH=$PATH:$HOME/bin
  kubectl version
  
  **Install EKS package on ubuntu **
  
  curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
  mv /tmp/eksctl /usr/local/bin
  eksctl version
  
  **INSTALL aws efs-ecs driver**
  
  **create EKS cluster**

     cat cluster.yaml

     eksctl create cluster -f cluster.yaml


  **create ConfigMap | StorageClass | PersistentVolume | PersistentVolumeClaim | Deployment**
  
     cat pg-deployment.yaml
     kubectl apply -f pg-deployment.yaml
     

