# EKS-Management
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

Grafana:
-------
It is a tool for creating and managing dashboards, alerts, reports, and other alarms.

ConfigMaps:
----------
Configmap is an API object used to store non-confidential data in key-value pairs. PODs can consume configMaps as evnvironment varibles

Secrets:
-------
A secret is an Object that contain a small amount of sensitive data such as passwords, tokens & keys.

Advantages:
- Scalability: Easily scale applications horizontally by adding more instances of pods.
- Reliability: Automatically restarts and replaces failed containers, ensuring applications are always running.
- Portability: Applications can run consistently across different environments, including on-premises and cloud platforms.
- Extensibility: Kubernetes supports custom extensions and integrations with other tools and services.
- Resource Optimization: Efficiently utilizes resources, running workloads based on available resources and constraints.

Disadvantages:
- Complexity: Kubernetes can be complex to set up and manage, especially for beginners.
- Overhead: Running a Kubernetes cluster introduces additional overhead compared to simpler container orchestration solutions.
- Steep Learning Curve: Understanding the various components and best practices requires time and effort.
