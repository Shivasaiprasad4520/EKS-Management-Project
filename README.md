# EKS-Management Project

Creating Kubernetcs-Cluster Management with Prometheus and Grafana
EKS Cluster Setup:
-----------------
Pre-Requisites:
1) Management Server with t2.micro
2) Cluster(t2.medium servers)

Helm: Package manager
----
Helm is a tool that helps you to manage Kubernetes applications with charts

EX: In Linux yum & apt-get
Prometheus:
-----------
Prometheus it is an open-source systems monitoring and alerting tool kit that collects and stores time series data of numeric metrics
![access prometheus](https://github.com/user-attachments/assets/f9f3176f-00c5-49ab-a760-4bc9e4fe22cb)


Grafana:
-------
It is a tool for creating and managing dashboards, alerts, reports, and other alarms.
![grafana](https://github.com/user-attachments/assets/8562d746-126d-44ea-8b0e-5c79bdf6bf1b)

ConfigMaps:
----------
Configmap is an API object used to store non-confidential data in key-value pairs. PODs can consume configMaps as evnvironment varibles

Secrets:
-------
A secret is an Object that contain a small amount of sensitive data such as passwords, tokens & keys.

------------------------------------------------------------------------------------
EKS Cluster Setup:
-----------------
Pre-Requisites:
1) Management Server with t2.micro
2) Cluster(t2.medium servers)
![creating cluster](https://github.com/user-attachments/assets/239b0905-d747-4deb-9460-403df47fe789)
Step 1 : Create EKS Management Host in AWS
-------
Launch new Ubuntu VM using AWS Ec2 ( t2.micro ) with ALLTCP

Step - 2 : Create IAM role & attach to EKS Management Host
---------
Create New Role using IAM service ( Select Usecase - ec2 )

Step - 3 : Create EKS Cluster using eksctl
============================================
Syntax:

eksctl create cluster --name cluster-name
--region region-name
--node-type instance-type
--nodes-min 2
--nodes-max 2 \ --zones,

![pods](https://github.com/user-attachments/assets/a614e390-bedc-4136-a0c8-ab19430af1ef)


Advantages:
----------
- Scalability: Easily scale applications horizontally by adding more instances of pods.
- Reliability: Automatically restarts and replaces failed containers, ensuring applications are always running.
- Portability: Applications can run consistently across different environments, including on-premises and cloud platforms.
- Extensibility: Kubernetes supports custom extensions and integrations with other tools and services.
- Resource Optimization: Efficiently utilizes resources, running workloads based on available resources and constraints.

Disadvantages:
-------------
- Complexity: Kubernetes can be complex to set up and manage, especially for beginners.
- Overhead: Running a Kubernetes cluster introduces additional overhead compared to simpler container orchestration solutions.
- Steep Learning Curve: Understanding the various components and best practices requires time and effort.
