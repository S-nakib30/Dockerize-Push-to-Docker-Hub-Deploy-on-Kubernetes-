Project : Dockerize, Push to Docker Hub & Deploy on Kubernetes (AWS EC2)

github: https://github.com/roy35-909/RapidCompetitions

Objective:

For The given GitHub repository link. Your task is to:

Dockerize the application

Push the image to Docker Hub

Set up a Kubernetes cluster on an AWS EC2 t3.medium instance

Deploy the application into the production namespace

 
Task Breakdown

1. Clone the Repository

Clone the given GitHub repository to your local machine.

 
 2. Dockerize the Application

Write a Dockerfile to containerize the app.

Build the Docker image locally.

Test the Docker container on your local machine to ensure it works.

 
3. Push to Docker Hub

Create a Docker Hub account (if not already available).

Tag the Docker image correctly.

Push the image to your Docker Hub repository.

 
4. Provision AWS EC2 Instance

Launch a t3.medium instance on AWS.

Ensure security group allows SSH (port 22) and Kubernetes-related ports (6443, 30000-32767).

 
5. Install Kubernetes Tools

SSH into the EC2 instance.

Install:

Docker

kubeadm, kubectl, kubelet

Initialize a single-node Kubernetes cluster using kubeadm.

Set up kubectl to interact with the cluster.

 
6. Create the Production Namespace

Create a namespace named production.

 
7. Deploy the Application

Write a Kubernetes Deployment manifest for the application.

Ensure it pulls the Docker image from your Docker Hub.

Apply the deployment to the production namespace.

Expose the application using a Service (e.g., ClusterIP, NodePort, or LoadBalancer).

 
 8. Verification

Check if the pods are running in the production namespace.

Confirm the application is accessible if exposed via NodePort or LoadBalancer.
