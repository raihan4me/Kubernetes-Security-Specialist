# Kubernetes-Security-Specialist
Scenario. You have joined the platform team at ShopFast, a small e-commerce company. The development team has been running an internal Kubernetes cluster with default settings. A recent internal review found these problems:

Nobody knows whether the control plane follows the CIS Benchmark.
Secrets are stored in plain text in etcd, and nothing records who changes what.
Every developer uses the cluster-admin kubeconfig.
Pods run as root, and any pod can talk to any other pod.
Images are pulled without being scanned or signed.
Nothing would notice an attacker opening a shell inside a container.

Your job is to build a reference "hardened" cluster that the team can copy. You will use kind (Kubernetes in Docker) on a single Ubuntu server and work through the main CKS (Certified Kubernetes Security Specialist) domains: cluster setup, cluster hardening, system hardening, minimising microservice vulnerabilities, supply chain security, and monitoring, logging and runtime security.

Learning Objectives
By the end of this lab you will be able to:

Build a kind cluster with a custom CNI (Calico), API server audit logging and Secret encryption at rest, and prove that each one works.

Run a CIS Kubernetes Benchmark scan with kube-bench, read the results and fix a failing control on a static-pod control plane.

Issue a client certificate through the Kubernetes CSR API, bind users, groups and ServiceAccounts to least-privilege Roles, and test access with kubectl auth can-i and raw API calls.

Enforce the Pod Security Standards restricted profile and write workloads that comply with it.
Write default-deny and allow-list NetworkPolicies and troubleshoot blocked traffic, including DNS.

Write admission policies in Rego (Gatekeeper) and in YAML (Kyverno), using both Audit and Enforce modes.

Scan images and manifests with Trivy, score manifests with kubesec, and sign and verify images with cosign.

Deploy Falco with the modern eBPF driver, write a custom rule, trigger detections, and investigate API activity in the audit log with jq.

