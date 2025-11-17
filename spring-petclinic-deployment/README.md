# Petclinic on VMware VMs with Jenkins & Ansible

## What This Project Does
- Builds and deploys the official Petclinic Java app to two VMs on VMware
- Uses Jenkins to automate the flow
- Uses Ansible to set up both Web and DB environments end-to-end

## Folder Structure
See above. Petclinic source lives in `spring-petclinic/`.

## Step-by-Step:
1. **Create 2 VMs in VMware** (Ubuntu recommended)
2. **Edit `ansible/inventory`** with each VM's IP
3. **Ensure SSH access** from Jenkins server to both VMs
4. **Set up Jenkins** with SSH credentials and Ansible plugin
5. **Run Jenkins pipeline** (copies app, provisions VMs, starts app)
6. **Result:** Petclinic app running at `http://YOUR_WEB_VM_IP:8080/`

## How to Build/Start Manually On VM

