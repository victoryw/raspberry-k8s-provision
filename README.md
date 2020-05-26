# Install k8s on raspberry pi
Use the 4 pis as server
* node is [raspberry pi 3B](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/) + 64GB SD
  * pi1
  * pi2
  * pi3
* master is （raspberry pi 4B 4GB)[https://www.raspberrypi.org/products/raspberry-pi-4-model-b/] + 64GB SD
  * pi4

## Server provisioning
* Raspberry Buster is support version 
* use the ali cloud source mirror as apt, docker image and Kubernetes
* install docker as container runtime
* install python3 and pip3 as the default python runtime
* install the full vim instead of vim common
* install kubeadm, etcd, kubelet and so on of the kubernate components


## Architecture
![](./.github/k8s.png)

## How to use
* This repo is composed of Ansible, Bash
* The python version is 3.7.7
* Please install [pipenv](https://github.com/pypa/pipenv)
* Setup the repo by pipenv install
* Setup the command line by pipenv run **ansbile commad**

## Others
* System setup, 
  which is about Raspberry pi server OS, hostname, ssh and so on, is on the [raspberry-os-self-setting-image](https://github.com/victoryw/raspberry-os-self-setting-image).
  This repo will resolve the problem of how automate burn os, and setup the hostname, ssh and so on.
* Todo:
  * upgrade the master to cluster
