# Complete CI/CD with Terraform

**Technologies used:**

Terraform, Jenkins, Docker, AWS, Git, Java, Maven, Linux, Docker Hub



**Project Description:**

Integrated provisioning stage into complete CI/CD Pipeline to automate provisioning server instead of
deploying an existing server

- Created SSH Key Pair

- Installed Terraform inside Jenkins container

- Added Terraform configuration to application’s git repository

- Adjusted Jenkinsfile to add “provision” step to the CI/CD pipeline that provisions EC2 instance

So the complete CI/CD project has the following configuration:

* CI step: Build artifact for Java Maven application

* CI step: Build and push Docker image to Docker Hub

* CD step: Automatically provision EC2 instance using TF

* CD step: Deploy new application version on the provisioned EC2 instance with Docker Compose
