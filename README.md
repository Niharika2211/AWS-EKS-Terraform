 1  wget -O - https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
    2  echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(grep -oP '(?<=UBUNTU_CODENAME=).*' /etc/os-release || lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
    3  sudo apt update && sudo apt install terraform
    4  terraform -version
    5  nano main.tf
    6  ls
    7  vim output.tf
    8  ls
    9  vim variable.tf
   10  ls
   11  terraform init
   12  ls
   13  terraform validate
   14  terraform plan
   15  curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
   16  unzip awscliv2.zip
   17  sudo ./aws/install
   18  apt install unzip
   19  aws configure
   20  apt install awscli
   21  curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
   22  unzip awscliv2.zip
   23  sudo ./aws/install
   24  aws configure
   25  terraform plan
   26  terraform apply
   27  terraform plan -var="ssh_key_name=k8s-key.ppk"
   28  terraform apply
   29  terraform apply -var="ssh_key_name=k8s-key.ppk"
   30  terraform apply -var="ssh_key_name=k8s-key"
   31  kubectl get svc -n monitoring kube-prometheus-stack-grafana
   32  curl -LO https://dl.k8s.io/release/v1.31.0/bin/linux/amd64/kubectl
   33  sudo chmod +x ./kubectl
   34  sudo mv kubectl /usr/local/bin
   35  kubectl version
   36  kubectl get svc -n monitoring kube-prometheus-stack-grafana
   37  aws eks update-kubeconfig --name eks-monitoring-demo-eks --region us-east-1
   38  kubectl get svc -n monitoring kube-prometheus-stack-grafana
   39  history
