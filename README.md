# Kubernetes Deployment

Setup kubernetes cluster with dashboard

## Getting Started

Download the project to your local workspace on ansible server, update hosts file with required master and slave nodes.
```
Example:
[allnodes]
icloudnow001
icloudnow002
```
By default icloudnow001 is the master node.

update aws.yml file with required image,user and key file details.
keyfile location is {{ proj }}/keyfiles/id_rsa.pub


### Prerequisites

ansible 


```
Redhat:
sudo yum install ansible

Centos:
sudo apt-get install ansible
```

### Installing
ansible-playbook -i "<path to inventory file>" -e "mode=apply cloud=aws proj=<path to your workspace project> env=aws" <path to playboook cloudnow.yml>

## Authors
IcloudNow


## License

License file for details
