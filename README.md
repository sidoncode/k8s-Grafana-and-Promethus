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
