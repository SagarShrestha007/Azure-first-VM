# Azure Free Tier VM Portfolio

This project demonstrates creating an "Azure Free Tier Virtual Machine (VM)" and hosting a "custom Nginx web server".  

## Live Demo
Since the VM is deleted, you can view the HTML locally or deploy a new VM.

## Features
- Free Tier Azure VM (B2as_v2)
- Ubuntu 22.04 LTS
- SSH access with SSH key
- Nginx web server with custom HTML page
- Basic Azure monitoring overview
- Auto-shutdown enabled to save costs

## File Structure
- `index.html` → Custom portfolio webpage  
- `screenshots/` → Placeholder for images (e.g., Nginx page)  
- `docs/VM_setup.md` → Detailed steps for VM creation  

## Setup Summary
1. Create Azure Free Tier VM (Ubuntu 22.04 LTS)  
2. Open ports: SSH (22) + HTTP (80)for nginx  
3. Connect via SSH  
ssh -i "PEM File path" azureuser@2VM's public IP address

4. Install Nginx:
```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx
