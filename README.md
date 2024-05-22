# Setup "nginx:latest"  docker  on AWS ECS such that I am able to access nginx index.html from a ALB
The flow of traffic is as follows

http:// ---> AWS-ECS: ---> nginx_docker:default_port
## Configure AWS account with aws-cli
1) aws configure
2) enter access key and secret access key
## Steps to launch server
1) terraform init
2) terraform plan -out nginx
3) terraform apply nginx

## Access the server
http://<load_balancer_dns_name>
