# Setup "nginx:latest"  docker  on AWS ECS such that I am able to access nginx index.html from a ALB
The flow of traffic is as follows

http:// ---> AWS-ECS: ---> nginx_docker:default_port
