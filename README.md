# 🚀 Terraform + Ansible VM Deployment Challenge

## 📋 Overview

This project demonstrates infrastructure automation by:
1. 🖥️ Deploying two Ubuntu virtual machines using **Terraform**.
2. ⚙️ Configuring **Nginx** web servers using **Ansible**.
3. 🌐 Serving a "Hello World" webpage accessible from the internet.

## 📌 Prerequisites

Before running this project, ensure you have the following installed:

- [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/index.html)
- [VirtualBox](https://www.virtualbox.org/) 
- [Vagrant](https://developer.hashicorp.com/vagrant/downloads) 
## 🚧 Challenges

### 1) Choosing a Hypervisor
**Challenge**: Selecting a hypervisor that is:
- Free
- Works on Windows/WSL (my PC setup) 
- Easy to test locally (reviewers should test with a single command, no complex configurations)

**Alternative Solutions Considered**:
| Option       | Why Not Chosen |
|--------------|----------------|
| **Proxmox**  | like using a rocket launcher to kill a mosquito we only have two lightweight VMs |
| **Cloud Solutions** (AWS/GCP/Azure) | Require account setup and might introduce costs|
| **Docker**   | Doesn't fully replicate VM environment |

**✅ Chosen Solution**: Vagrant + VirtualBox  
**Reasons**:
- No costs involved, perfect for local development.
- Works offline, no online dependencies needed.
- And it works on Windows, macOS, and Linux without requiring cloud resources
- Via Vagrant VirtualBox is compatible with Terraform

### 2) ...
...