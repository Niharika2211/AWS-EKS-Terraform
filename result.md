Outputs:

bastion_public_ip = "3.92.188.180"
eks_cluster_name = "eks-monitoring-demo-eks"
grafana_service_hint = "Use: kubectl get svc -n monitoring kube-prometheus-stack-grafana"
private_subnets = [
  "subnet-0a85e8efdd744d7ff",
  "subnet-0c7f28ef667722201",
  "subnet-0e9cfc7acbdc369d9",
]
public_subnets = [
  "subnet-0f19fa71893e47d4f",
  "subnet-07a9106773e221c6f",
  "subnet-09bd35ff36a1f4a3b",
]
vpc_id = "vpc-01649de88ce12452a"


root@ip-172-31-70-115:~# kubectl get svc -n monitoring kube-prometheus-stack-grafana
NAME                            TYPE           CLUSTER-IP       EXTERNAL-IP                                                              PORT(S)        AGE
kube-prometheus-stack-grafana   LoadBalancer   172.20.126.123   af371df7d96434e04af3f10962cb96d0-613570318.us-east-1.elb.amazonaws.com   80:30353/TCP   29m

