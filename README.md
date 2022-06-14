# Jenkins provisioning with Vagrant and Ansible
Spin up a Jenkins test instance with vagrant and Ansible 👷🔧👷 

## Abstract
Jenkins is an open source automation server.
<br>
It helps automate the parts of software development related to building, testing, and deploying, facilitating
continuous integration and continuous delivery.

This repository contains IaC scripts for provisioning a local Jenkins instance via Vagrant and Ansible.

## Instructions
clone this repo:
```console
git clone https://github.com/R3DRUN3/jenkins-ansible-provisioning.git \
&& cd jenkins-ansible-provisioning
```
fire up the provisioning:
```console
vagrant up
```
when finished, open a browser to access the Jenkins web UI and follow the instructions for configuration:
```console
firefox 192.168.56.10:8080
```
## Test Jobs and CI/CD pipelines
This repo also contain a simple flask web app that you can use to test Jenkins pipelines,
for example you can set up a Jenkins Build with the Snyk plugin for software vulnerability assessment:

![alt_text](https://github.com/R3DRUN3/jenkins-ansible-provisioning/blob/main/app/images/snyk-pipeline.png)



