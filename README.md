Setup Jenkins and Kubernetes on AWS using Ansible

# Steps

## Copy var_sample.yaml to vars.yaml

## Jenkins infrastructure on AWS 

### Setup

`` ansible-playbook setup-infra.yaml -vvv ``
`` ansible-playbook start-docker-jenkins-container.yaml -vvv ``

### Teardown

`` ansible-playbook teardown-infra.yaml -vvv; ``

## Kubernetes cluster using kops on AWS

### Setup

`` ansible-playbook setup-k8s-cluster-aws-kops.yaml -vvv ``

### Teardown

`` ansible-playbook teardown-k8s-cluster-aws-kops.yaml -vvv ``

## Please ensure the AWS configure setup is done prior to running ansible