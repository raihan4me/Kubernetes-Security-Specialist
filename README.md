# Kubernetes-Security-Specialist
Scenario. You have joined the platform team at ShopFast, a small e-commerce company. The development team has been running an internal Kubernetes cluster with default settings. A recent internal review found these problems:

Nobody knows whether the control plane follows the CIS Benchmark.
Secrets are stored in plain text in etcd, and nothing records who changes what.
Every developer uses the cluster-admin kubeconfig.
Pods run as root, and any pod can talk to any other pod.
Images are pulled without being scanned or signed.
Nothing would notice an attacker opening a shell inside a container.

Your job is to build a reference "hardened" cluster that the team can copy. You will use kind (Kubernetes in Docker) on a single Ubuntu server and work through the main CKS (Certified Kubernetes Security Specialist) domains: cluster setup, cluster hardening, system hardening, minimising microservice vulnerabilities, supply chain security, and monitoring, logging and runtime security.
