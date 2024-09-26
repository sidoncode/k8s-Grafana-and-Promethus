# K8s Grafana and Promethus


## Steps for the Tutorial:

### Create IAM User and Configure aws cli , eksctl and kubectl in ec2 / local machine

### >> aws configure >> region / json / Key(Access and Secret Key)

### >> eksctl create cluster --name my-k8s-cluster --region us-east-1 --nodes 2 --node-type t3.medium 

### >> git clone https://github.com/sidoncode/k8s-Grafana-and-Promethus

### >> kubectl create -f 1-prometheus/. 

### >> kubectl create -f 2-grafana/. 

### >> kubectl get all -n monitoring 

### >> kubectl rollout restart deployment coredns -n kube-system 

### >> Click on Import Dashboard by clicking on + sign from top right corner. 

### >> For Find and Import dashboards, Enter 6417, and Click on Load.


<br>

 1001  aws configure
 1002  eksctl create cluster --name my-k8s-cluster --region us-east-1 --nodes 2 --node-type t3.medium 
 1003  kubectl get nodes
 1004  git clone https://github.com/sidoncode/k8s-Grafana-and-Promethus
 1005  cd k8s-Grafana-and-Promethus
 1006  ls -l
 1007  kubectl create -f 1-prometheus
 1008  kubectl create -f 2-grafana
 1009  kubectl get all -n monitoring
 1010  kubectl get svc _A
 1011  kubectl get svc -A
 1012  ssh -i "id_rsa" root@ec2-44-211-83-206.compute-1.amazonaws.com ec2metadata --public-ipv4
 1013  ssh -i "id_rsa" root@ec2-44-211-83-206.compute-1.amazonaws.com ec2metadata --public-ipv4
 1014  ssh -i "id_rsa" root@ec2-44-211-83-206.compute-1.amazonaws.com ec2metadata --public-ipv4
 1015  kubectl rollout restart deployment coredns -n kube-system 
 1016  kubectl get svc -A
