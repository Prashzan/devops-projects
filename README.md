# DevOps Portfolio – Prashant Bhattarai

## About Me
DevOps & Cloud Engineer with hands-on experience in AWS, Docker, Kubernetes,
Terraform, Jenkins, Ansible, and monitoring tools.

---

## 🔧 DevOps Projects

### 1. Dockerizing-js-app 
**Tools:** Docker, Amazon ECR, Node.js, MongoDB, MongoExpress  

**Project Description:**  
1. Copy Docker-compose file to remote server
2. Login to private Docker registry on remote server to
fetch our app image
3. Start our application container with MongoDB and
4. MongoExpress services using docker compose

🔗 Repo: https://github.com/Prashzan/dockerizing-js-app

---

### 2. Jenkins-Shared-Library
**Tools:** Groovy, Java, Jenkins, Groovy, Docker, Maven

**Project Description:**  
1. Create a Jenkins Shared Library to extract common build
logic:
2. Create separate Git repository for Jenkins Shared
Library project
3. Create functions in the JSL to use in the Jenkins pipeline
4. Integrate and use the JSL in Jenkins Pipeline (globally and
for a specific project in Jenkinsfile)

🔗 Repo: https://github.com/Prashzan/jenkins-shared-library

---


### 3. Deploy to ec2 using jenkins pipeline
**Tools:** AWS, Jenkins, Docker, Linux, Git, Java, Maven, Docker Hub 

**Project Description:**  
1. Prepare AWS EC2 Instance for deployment (Install Docker)
2. Create ssh key credentials for EC2 server on Jenkins
3. Extend the previous CI pipeline with deploy step to ssh into the
remote EC2 instance and deploy newly built image from Jenkins
server
4. Configure security group on EC2 Instance to allow access to our
web application
5. Install Docker Compose on AWS EC2 Instance
6. reate docker-compose.yml file that deploys our web
application image
7. onfigure Jenkins pipeline to deploy newly built image
using Docker Compose on EC2 server
8. Improvement: Extract multiple Linux commands that
are executed on remote server into a separate shell
script and execute the script from Jenkinsfile

🔗 Repo: https://github.com/Prashzan/deploy-to-ec2-using-jenkins-pipeline

---

### 4. Deploy mongodb and mongo express in local kubernetes cluster
**Tools:** Kubernetes, Docker, MongoDB, Mongo Express  

**Project Description:**  
1. Setup local K8s cluster with Minikube
2. Deploy MongoDB and MongoExpress with
configuration and credentials extracted into
ConfigMap and Secret
🔗 Repo: https://github.com/Prashzan/mongodb-with-mongoexpress-in-kubernetes

---

### 5. Deploy microservices in linode kubernetes cluster with Helm charts
**Tools:** Kubernetes, Redis, Linux, Linode LKE, Helm, Helmfile

**Project Description:**  
1. Create K8s manifests for Deployments and Services
for all microservices of an online shop application
2. Deploy microservices to Linode’s managed Kubernetes
cluster
3. Create 1 shared Helm Chart for all microservices, to reuse
common Deployment and Service configurations for the services
4. Deploy Microservices with Helm
5. Deploy Microservices with Helmfile

🔗 Repo: https://github.com/Prashzan/deploy-microservices-linode

---

### 6. Deploy to eks cluster using jenkins pipeline
**Tools:** Kubernetes, Jenkins, AWS EKS, Docker Hub, Java, Maven, Linux, Docker,Git  

**Project Description:**  
1. Install kubectl and aws-iam-authenticator on a Jenkins
server
2. Create kubeconfig file to connect to EKS cluster and
add it on Jenkins server
3. Add AWS credentials on Jenkins for AWS account
authentication
4. Extend and adjust Jenkinsfile of the previous CI/CD
pipeline to configure connection to EKS cluster
5. Write K8s manifest files for Deployment and Service configuration
6. Integrate deploy step in the CI/CD pipeline to deploy newly built application image from
DockerHub private registry to the EKS cluster
So the complete CI/CD project we build has the following configuration:
  - CI step: Increment version
  - CI step: Build artifact for Java Maven application
  - CI step: Build and push Docker image to DockerHub
  - CD step: Deploy new application version to EKS cluster
  - CD step: Commit the version update

🔗 Repo: https://github.com/Prashzan/deploy-to-eks-cluster-jenkins-pipeline

---

### 7. Automate Provisioning of EC2 Instance with Terraform
**Tools:** Terraform, AWS, Docker, Linux, Git 

**Project Description:**  
1. Create TF project to automate provisioning AWS Infrastructure
and its components, such as: VPC, Subnet, Route Table, Internet
Gateway, EC2, Security Group
2. Configure TF script to automate deploying Docker container to
EC2 instance

🔗 Repo: https://github.com/Prashzan/automate-provisioning-ec2--terraform

---

### 8. Provisioning of EKS cluster with Terraform using modules
**Tools:** Terraform, AWS EKS, Docker, Linux, Git  

**Project Description:**  
1. Automate provisioning EKS cluster with Terraform

🔗 Repo: https://github.com/Prashzan/eks-provisioning-terraform

---

### 9. Complete CI/CD with Terraform
**Tools:** Terraform, Jenkins, Docker, AWS, Git, Java, Maven, Linux, Docker Hub  

**Project Description:**  
1. Integrate provisioning stage into complete CI/CD Pipeline to automate provisioning server instead of deploying to an existing server
2. Create SSH Key Pair
3. Install Terraform inside Jenkins container
4. Add Terraform configuration to application’s git repository
5. Adjust Jenkinsfile to add “provision” step to the CI/CD pipeline that provisions EC2 instance
So the complete CI/CD project we build has the following configuration:
- CI step: Build artifact for Java Maven application
- CI step: Build and push Docker image to Docker Hub
- CD step: Automatically provision EC2 instance using TF
- CD step: Deploy new application version on the provisioned EC2 instance with Docker Compose

🔗 Repo: https://github.com/Prashzan/ci-cd-terraform-jenkins

---

### 10. Automation with Python
**Tools:** Python, Linode, Docker, Linux, Boto3, AWS  

**Project Description:**  
1. Create EC2 Instances with Terraform
2. Python script that fetches statuses of EC2
Instances and prints to the console
3. Extend the Python script to continuously check the status
of EC2 Instances in a specific interval
4. Python script that automates adding
environment tags to all EC2 Server instances
5. Python script that fetches and displays EKS cluster
status and information
6. Python script that automates creating backups
for EC2 Volumes
7. Python script that cleans up old EC2 Volume
snapshots
8. Python script that restores EC2 Volumes
9. Create a server on a cloud platform
10. Install Docker and run a Docker container on the remote server
11. Python script that monitors the website by accessing it and validating the
HTTP response
12. Python script that sends an email notification when website is down
13. Python script that automatically restarts the application & server when
the application is down

🔗 Repo: https://github.com/Prashzan/python-automation-on-aws-and-linode

---

### 11. Deployments using ansible
**Tools:** Ansible, Node.js, DigitalOcean, Linux, Java, Nexus, AWS, Terraform, Docker

**Project Description:**  
1. Create Server on DigitalOcean
2. Write Ansible Playbook that installs necessary
technologies, creates Linux user for an application and
deploys a NodeJS application with that user
3. Write Ansible Playbook that creates Linux user for Nexus,
configure server, installs and deploys Nexus and verifies
that it is running successfully
4. Create AWS EC2 Instance with Terraform
5. Write Ansible Playbook that installs necessary
technologies like Docker and Docker Compose, copies
docker-compose file to the server and starts the
Docker containers configured inside the docker-
compose file
6. Create Ansible Playbook for Terraform integration
7. Adjust Terraform configuration to execute Ansible
Playbook automatically, so once Terraform provisions a
server, it executes an Ansible playbook that configures
the server

🔗 Repo: https://github.com/Prashzan/ansible_deployments

---

### 12. Automate Kubernetes Deployment using Ansible

**Tools:** Ansible, Terraform, Kubernetes, AWS EKS, Python, Linux  
**Project Description:**  
1. Create EKS cluster with Terraform
2. Write Ansible Play to deploy application in a new K8s
namespace
🔗 Repo: https://github.com/Prashzan/deploy-in-eks-using-ansible
---

### 13. Complete CI/CD Jenkins Pipeline with Ansible Integration
**Tools:** KubAnsible, Jenkins, DigitalOcean, AWS, Boto3, Docker, Java, Maven, Linux, Git  

**Project Description:**  
1. Create and configure a dedicated server for Jenkins
2. Create and configure a dedicated server for Ansible Control Node
3. Write Ansible Playbook, which configures 2 EC2 Instances
4. Add ssh key file credentials in Jenkins for Ansible Control Node server and Ansible Managed Node
servers
5. Configure Jenkins to execute the Ansible Playbook on remote Ansible Control Node server as
part of the CI/CD pipeline
So the Jenkinsfile configuration will do the following:
- Connect to the remote Ansible Control Node server
- Copy Ansible playbook and configuration files to the remote Ansible Control Node server
- Copy the ssh keys for the Ansible Managed Node servers to the Ansible Control Node server
- Install Ansible, Python3 and Boto3 on the Ansible Control Node server
- With everything installed and copied to the remote Ansible Control Node server, execute the
playbook remotely on that Control Node that will configure the 2 EC2 Managed Nodes

🔗 Repo: https://github.com/Prashzan/integrate-ansible-with-jenkins-pipeline

---

### 14. Install prometheus stack on kubernetes, configure Alerting for our applicaion and monitoring for a 3rd party applicaion 
**Tools:** Prometheus, Kubernetes, Helm, AWS EKS, eksctl, Grafana, Linux, Redis  

**Project Description:**  
1. Setup EKS cluster using eksctl
2. Deploy Prometheus, Alert Manager and Grafana in cluster as
part of the Prometheus Operator using Helm chart
3. Configure our Monitoring Stack to notify us whenever
CPU usage > 50% or Pod cannot start
- Configure Alert Rules in Prometheus Server
- Configure Alertmanager with Email Receiver
4. Monitor Redis by using Prometheus Exporter
- Deploy Redis service in our cluster
- Deploy Redis exporter using Helm Chart
- Configure Alert Rules (when Redis is down or has too many
connections)
- Import Grafana Dashboard for Redis to visualize monitoring
data in Grafana

🔗 Repo: https://github.com/Prashzan/monitoring-and-alert-files

---

### 15. Monitoring our custom nodejs app using prometheus
**Tools:** Prometheus, Kubernetes, Node.js, Grafana, Docker, Docker Hub 

**Project Description:**  
1. Configure our NodeJS application to collect &
expose Metrics with Prometheus Client Library
2. Deploy the NodeJS application, which has a metrics
endpoint configured, into Kubernetes cluster
3. Configure Prometheus to scrape this exposed
metrics and visualize it in Grafana Dashboard

🔗 Repo: https://github.com/Prashzan/monitoring-nodejs-app-using-prometheus

---
